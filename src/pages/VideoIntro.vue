<template>
    <Layout>
        <section class="s-content s-content--single">
            <div class="row">
                <div class="column large-12">

                    <article class="s-post entry format-audio">

                        <div class="s-content__media">
                            <div class="video-container">
                                <iframe width="640" height="360" src="https://www.youtube.com/embed/zAP7HxAmygg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                            </div>
                        </div> <!-- end s-content__media -->

                        <div class="s-content__primary">

                            <h2 class="s-content__title s-content__title--post">Introduction to Kubernetes.</h2>

                            <ul class="s-content__post-meta">
                                <li class="date">April 18, 2022</li>
                                <!-- <li class="cat"><a href="">Frontend</a><a href="">Design</a></li> -->
                            </ul>

                            <p class="lead">
                            Easily one of the best introduction videos for Kubernetes. Featuring Seth (on the left) and Brendan Burns, co-creator of kubernetes, now working as a distinguished developer at Microsoft.</p> 

                            <p>I came across this video when trying to skill up quickly, and found it probably one of the best videos out there to explain the concepts, especially if you've heard of / tried Docker already. One of the most amazing things about Microsoft videos (which I've watched for years at this point), is their ability to interview people who actually created the technology we're learning about. Here is no exception as Brendan explains all the concepts, but also some main benefits of kubernetes. Grab a coffee and enjoy the next 40 minutes - or add to your watch later queue. Trust me, it's worth the watch.
                            </p>
                        </div>

                    </article>
                    <!-- END respond-->
                </div> <!-- end comment-respond -->
            </div> <!-- end comments-wrap -->
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