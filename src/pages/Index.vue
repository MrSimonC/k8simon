<template>
  <Layout>
   
    <!-- masonry
    ================================================== -->
    <section class="s-bricks">

        <div class="masonry">
            <div class="bricks-wrapper h-group">
 
                <div class="grid-sizer"></div>

                <div class="brick entry featured-grid animate-this">
                    <div class="entry__content">

                        <div class="featured-post-slider">
                            
                            <CardFeatured
                                image="background-image:url('images/thumbs/featured/video-intro.jpg');"
                                date="18 April 2022"
                                author="Simon Crouch"
                                title="Introduction to Kubernetes Video"
                                link="/video-intro/"
                            />

                            <CardFeatured
                                image="background-image:url('images/thumbs/featured/chairs.jpg');"
                                date="16 April 2022"
                                author="Simon Crouch"
                                title="A Lesson in AKS Managed Identity"
                                link="/first-lesson/"
                            />

                        </div> <!-- end feature post slider -->
                        
                        <div class="featured-post-nav">
                            <button class="featured-post-nav__prev">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M12.707 17.293L8.414 13H18v-2H8.414l4.293-4.293-1.414-1.414L4.586 12l6.707 6.707z"></path></svg>
                            </button>
                            <button class="featured-post-nav__next">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M11.293 17.293l1.414 1.414L19.414 12l-6.707-6.707-1.414 1.414L15.586 11H6v2h9.586z"></path></svg>
                            </button>
                        </div> <!-- featured-post-nav -->

                    </div> <!-- end entry content -->
                </div> <!-- end entry, featured grid -->
 
                <CardStandard
                    title='A lesson in AKS and Managed Id' 
                    description='In my first blog, I learned about what Azure Kubernetes Service does when it creates a cluster. Also, I learned about Managed Identity and how to use it in AKS.'
                    link='/first-lesson/'>
                    <template slot="image">
                        <g-image src='~/../static/images/thumbs/featured/chairs.jpg' alt='A lesson in AKS and Managed Id'></g-image>
                    </template>
                </CardStandard>

                <CardVideo
                    title='Kubernetes Documentary' 
                    description='Watch how kubernetes was formed in the early days, featuring interviews with developers and key players.'
                    link='/video-documentary/'>
                    <template slot="image">
                        <g-image src='~/../static/images/thumbs/featured/video-documentary.jpg' alt='Kubernetes Documentary'></g-image>
                    </template>
                    </CardVideo>

                <CardQuote
                    quote='The inevitable trajectory of all software is death.'
                    author='Brendan Burns'
                    authortitle='Co-founder, Kubernetes'
                />

                <CardVideo
                    title='Introduction to Kubernetes' 
                    description='Featuring Brendan Burns, here is a great 40 minute video introduction to kubernetes.'
                    link='/video-intro/'>
                    <template slot="image">
                        <g-image src='~/../static/images/thumbs/featured/video-intro.jpg' alt='Introduction to Kubernetes'></g-image>
                    </template>
                </CardVideo>

                <CardVideo
                    title='Kubernetes Basics'
                    description='Learn more concepts about kubernetes in these short 5-minute long videos from Microsoft in this YouTube playlist.'
                    link='/video-basics-playlist/'>
                    <template slot="image">
                        <g-image src='~/../static/images/thumbs/masonry/video-basics-playlist.jpg' alt='Kubernetes Basics'></g-image>
                    </template>
                </CardVideo>
            </div> <!-- end brick-wrapper --> 
 
        </div> <!-- end masonry -->

        <div class="row">
            <div class="column large-12">
                <!-- <nav class="pgn">
                    <ul>
                        <li>
                            <a class="pgn__prev" href="#0">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M12.707 17.293L8.414 13H18v-2H8.414l4.293-4.293-1.414-1.414L4.586 12l6.707 6.707z"></path></svg>
                            </a>
                        </li>
                        <li><a class="pgn__num" href="#0">1</a></li>
                        <li><span class="pgn__num current">2</span></li>
                        <li><a class="pgn__num" href="#0">3</a></li>
                        <li><a class="pgn__num" href="#0">4</a></li>
                        <li><a class="pgn__num" href="#0">5</a></li>
                        <li><span class="pgn__num dots">…</span></li>
                        <li><a class="pgn__num" href="#0">8</a></li>
                        <li>
                            <a class="pgn__next" href="#0">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M11.293 17.293l1.414 1.414L19.414 12l-6.707-6.707-1.414 1.414L15.586 11H6v2h9.586z"></path></svg>
                            </a>
                        </li>
                    </ul>
                </nav> <-- end pgn -->
            </div> <!-- end column -->
        </div> <!-- end row -->
    </section> <!-- end s-bricks -->
  </Layout>
</template>

<script>
import CardStandard from '~/components/CardStandard.vue'
import CardVideo from '~/components/CardVideo.vue'
import CardQuote from '~/components/CardQuote.vue'
import CardFeatured from '~/components/CardFeatured.vue'

export default {
  metaInfo: {
    title: 'Learn about kubernetes',
    meta: [
        { author: 'simon crouch', description: 'Learn more about kubernetes, including videos, blog posts, and learnings from actual real-life development work in production.' }
    ]
  },
  components: {
    CardStandard,
    CardVideo,
    CardQuote,
    CardFeatured
  }
}
</script>
