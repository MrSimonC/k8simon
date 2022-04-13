<template>
  <Layout>
     <section class="s-content">
        <div class="row">
            <div class="column large-12">

                <section>

                    <div class="s-content__media">
                        <g-image src="~/../static/images/thumbs/about/about-1050.jpg" />
                    </div> <!-- end s-content__media -->

                    <div class="s-content__primary">

                        <h1 class="s-content__title">Hey there, I'm Simon.</h1>	

                        <p class="lead">Welcome to my site, all about kubernetes. I live in Bristol in the UK and have two very small exhausting children. I've always hated the idea of starting a blog, but having become a C# developer I've always discovered I've solved problems which are either unique to me & have no answer on the Internet or the answer is really hard to find...</p> 

                        <p>I started this site April 2022 after having joined a new company and worked there for under a year. The company I work for is moving fast in the digital space, however, it's new to many of them. Kubernetes included. </p>

                        <p>At the time of writing we are using Azure, and have a kubernetes cluster ready (Azure Kubernetes service – AKS), but not in production… Yet. Therefore I'm new, the company is new to this kind of thing, we have to push out production in a few months… And already I'm learning lessons faster than children run to an ice cream van! The idea is if I can help even one or two people out there, then I've done my job! If you are new to kubernetes, then welcome! If you've been doing this for awhile, then I hope you find at least something useful here!</p>

                        <hr>

                        <p>Starting this site I had a few rules.</p>

                        <div class="row block-large-1-2 block-tab-full s-content__blocks">
                            <div class="column">
                                <h4>Focused.</h4>
                                <p>I could totally tell you about my sleep deprivation from my small children or how hard they are trying to get out the house to Nursery and School, but I won't. I think we'd all much rather I stick to kubernetes!</p>
                            </div>

                            <div class="column">
                                <h4>Beautiful.</h4>
                                <p>I can't stand seeing another blog site where everything looks the same, and everybody copies and pastes the same style (WordPress has given us lots of good things, but a common theme for blogs is not one of them). This site should at least be visually engaging – and somewhere where you want to hang out at least! I used to create basic html websites back in the 90s & a little nostalgia never hurt anyone.</p>
                            </div>

                            <div class="column">
                                <h4>Experimental.</h4>
                                <p>I should at least try and experiment with this website – is basic HTML okay to log posts with? Do I need a content management system (like netlify CMS)? In a coffee shop I tried out HUGO, with GitHub, a Hugo theme, and Netlify CMS. The result was a very boring looking website which is easy for me to update. That's completely the wrong way round in my opinion – if I do have to choose, it should be hard for me to update but beautiful for you to read!</p>
                            </div>

                            <div class="column">
                                <h4>Blog From Anywhere.</h4>
                                <p>As any parent in my position (with young children) will know, time is of the essence always and having any kind of spare time is impossible. Anything goes – this entire page you are reading has been dictated while I was getting ready, then edited over breakfast, so if I can try and cram in anything in my busy life to get something up on the site, then it's gonna be worth trying!</p>
                            </div>
                        </div>

                    </div> <!-- end s-content__primary -->

                </section>

            </div> <!-- end column -->
        </div> <!-- end row -->
    </section> <!-- end s-content -->
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'About us'
  }
}
</script>
