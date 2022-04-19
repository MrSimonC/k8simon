<template>
    <Layout>
        <section class="s-content s-content--single">
            <div class="row">
                <div class="column large-12">

                    <article class="s-post entry format-audio">

                        <div class="s-content__media">
                            <div class="video-container">
                                <iframe width="640" height="360" src="https://www.youtube.com/embed/videoseries?list=PLLasX02E8BPCrIhFrc_ZiINhbRkYMKdPT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                            </div>
                        </div> <!-- end s-content__media -->

                        <div class="s-content__primary">

                            <h2 class="s-content__title s-content__title--post">Kubernetes Basics.</h2>

                            <ul class="s-content__post-meta">
                                <li class="date">April 19, 2022</li>
                                <!-- <li class="cat"><a href="">Frontend</a><a href="">Design</a></li> -->
                            </ul>

                            <p class="lead">
                            In this playlist of roughly 5-minute long videos from Microsoft, Brendan Burns explains the key concepts of Kubernetes. From why we should care about containers, to getting ready for production these videos give you a good set up from introductions to the subject.</p>

                            <p><a href="https://youtube.com/playlist?list=PLLasX02E8BPCrIhFrc_ZiINhbRkYMKdPT">⏯️ https://youtube.com/playlist?list=PLLasX02E8BPCrIhFrc_ZiINhbRkYMKdPT</a></p>

                            <p>Although these videos are slightly out of order, I have still bookmarked this playlist myself and dip into it now and again - it's really useful to remind myself of key concepts both in a general way, and when revisiting an area. Impressively Brendan is able to write backwards on a clear whiteboard which explaining the concepts - which is quite an impressive skill if you think about it.
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