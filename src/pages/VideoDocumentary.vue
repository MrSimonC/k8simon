<template>
    <Layout>
        <section class="s-content s-content--single">
            <div class="row">
                <div class="column large-12">

                    <article class="s-post entry format-audio">

                        <div class="s-content__media">
                            <div class="video-container">
                                <iframe width="640" height="360" src="https://www.youtube.com/embed/BE77h7dmoQU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                            </div>
                        </div> <!-- end s-content__media -->

                        <div class="s-content__primary">

                            <h2 class="s-content__title s-content__title--post">Kubernetes Documentary</h2>

                            <ul class="s-content__post-meta">
                                <li class="date">April 18, 2022</li>
                                <!-- <li class="cat"><a href="">Frontend</a><a href="">Design</a></li> -->
                            </ul>

                            <p class="lead">
                            Every wondered how kubernetes started? Who was involved? Check out the official kubernetes documentary on YouTube.</p> 

                            <p>Fascinating to see how kubernetes was formed, developed and welcomed (eventually) but the container-community. Great to hear from the key players, developers and find how it all started. This is part 1 of 2 videos. <a href="https://www.youtube.com/watch?v=318elIq37PE">Check out part 2 here.
                            </a></p>
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