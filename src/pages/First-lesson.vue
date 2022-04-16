<template>
    <Layout>
        <section class="s-content s-content--single">
            <div class="row">
                <div class="column large-12">

                    <article class="s-post entry format-standard">

                        <div class="s-content__media">
                            <div class="s-content__post-thumb">
                                <g-image src="~/../static/images/thumbs/masonry/chairs.jpg" alt="room2, southampton" />
                                <small>room2, Southampton</small>
                            </div>
                        </div>

                        <div class="s-content__primary">

                            <h2 class="s-content__title s-content__title--post">AKS Managed Id</h2>

                            <ul class="s-content__post-meta">
                                <li class="date">April 16, 2022</li>
                                <!-- <li class="cat"><a href="">AKS</a><a href="">Azure</a></li> -->
                            </ul>

                            <p class="lead">
                                Welcome to my first blog entry - but also the first lesson I learned about running kubernetes on Azure Kubernetes Service (AKS).</p> 

                            <p class="drop-cap">The absolute first thing you should know is that when you create an AKS, Microsoft will set up a few things they need to help look after your cluster. So as not to confuse you, Microsoft create an additional resource group alongside your own (I never even knew they did that, so initially I found it confusing. The irony). This is called “MC_yourResourceGroupName_yourClusterName_yourChosenLocation”.  This is the default notation, so be aware someone you work with may have renamed it / <a href="https://docs.microsoft.com/en-us/azure/aks/faq#can-i-provide-my-own-name-for-the-aks-node-resource-group">created it with a different name.</a>
                            </p>

                            <blockquote>
                                <p>
                                    “The second resource group, known as the node resource group, contains all of the infrastructure resources associated with the cluster.”
                                </p>
                                <cite><a href='https://docs.microsoft.com/en-us/azure/aks/faq#why-are-two-resource-groups-created-with-aks'>Microsoft Documentation</a></cite>
                            </blockquote>

                            <p>The situation I found myself in was that I had to work on an AKS which someone had already made. When creating the cluster, they had selected (unbeknownst to me) “managed system identity” authentication.
                            </p>

                            <p>What this does is created a new system managed identity called “yourAKSClusterName-agentpool”, and puts it in the “MC_…” node resource group we talked about above.</p>

                            <p>This managed identity is what you should be adding (on a basic level) to your other azure resources (key vaults, container registries etc) if you want things in your cluster to be able to access them.</p>

                            <p>At this point, most newbies can stop reading, as your basic kubernetes cluster can now access other azure resources if you add that managed id to those resources.</p>

                            <p>
                                <g-image src="~/../static/images/thumbs/masonry/chairs-drink.jpg" alt="room2, southampton" />
                            </p>

                            <h3>User Assigned Managed Identities</h3>

                            <p>When I started work on an existing AKS cluster, I started adding user assigned managed identities to my azure resources (key vaults etc), but couldn’t work out how to tie the user signed identities back to the (calling) cluster. There was just no connection between them. That yourAKSClusterName-agentpool was the secret sauce.</p>

                            <blockquote>
                                <p>
                                    “This auto-created “...-agentpool” managed identity represents your whole kubernetes cluster.”
                                </p>
                                <!-- <cite><a href='https://docs.microsoft.com/en-us/azure/aks/faq#why-are-two-resource-groups-created-with-aks'>Microsoft Documentation</a></cite> -->
                            </blockquote>

                            <p>However, what if you want a bit more granular control? What if each service (specifically pod) should really have their own identity?</p>

                            <p>Well, in terms of Azure managed identity with regard to pod specific identities, there is one main de facto library of time writing:</p>

                            <p><a href="https://github.com/Azure/aad-pod-identity">https://github.com/Azure/aad-pod-identity</a></p>

                            <p>This is an open source project, but with the backing of Microsoft. You can read about how to get started in the link.</p>
                            
                            <p>The future direction of doing pod based identity will be “workflow identities”. Think aad pod identity v2. At time of writing (April 2022), managed identities are not currently supported in the new “workflow identity” - as it’s just too early days, but are for the existing aad-pod-identity … 
                            </p>

                            <p>Not having managed identity support is a dealbreaker for us on our project using Azure - so we’ll stick to the aad pod identity.</p>

                            <p>My thanks to the Finland Azure user group Who did talk on the subject and is definitely worth a watch: <a href="https://youtu.be/c4C9FnI4ZPw">https://youtu.be/c4C9FnI4ZPw</a></p>

                            <p>I hope this provides a little illumination for those of you getting started… It definitely caught us out. Hopefully reading this I’ve saved somebody else the hard lesson we had to learn!</p>
                        </div>
                    </article>
                </div>
                <Author />
            </div>


        </section>
    </Layout>
</template>

<script>
    import Author from '~/components/Author.vue'

    export default {
        components: {
        Author
        }
    }
</script>