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

                        <p class="lead">Welcome to my site, all about kubernetes. I live in Bristol in the UK and have two very small exhausting children. I’ve always hated the idea of starting a blog, but having become a C# developer I’ve always discovered I’ve solved problems which are either unique to me & have no answer on the Internet or the answer is really hard to find...</p> 

                        <p>I started this site April 2022 after having joined a new company and worked there for under a year. The company I work for is moving fast in the digital space, however, it’s new to many of them. Kubernetes included. </p>

                        <p>At the time of writing we are using Azure, and have a kubernetes cluster ready (Azure Kubernetes service – AKS), but not in production… Yet. Therefore I’m new, the company is new to this kind of thing, we have to push out production in a few months… And already I’m learning lessons faster than children run to an ice cream van! The idea is if I can help even one or two people out there, then I’ve done my job! If you are new to kubernetes, then welcome! If you’ve been doing this for awhile, then I hope you find at least something useful here!</p>

                        <hr>

                        <p>Starting this site I had a few rules.</p>

                        <div class="row block-large-1-2 block-tab-full s-content__blocks">
                            <div class="column">
                                <h4>Focused.</h4>
                                <p>I could totally tell you about my sleep deprivation from my small children or how hard they are trying to get out the house to Nursery and School, but I won’t. I think we’d all much rather I stick to kubernetes!</p>
                            </div>

                            <div class="column">
                                <h4>Beautiful.</h4>
                                <p>I can’t stand seeing another blog site where everything looks the same, and everybody copies and pastes the same style (WordPress has given us lots of good things, but a common theme for blogs is not one of them). This site should at least be visually engaging – and somewhere where you want to hang out at least! I used to create basic html websites back in the 90s & a little nostalgia never hurt anyone.</p>
                            </div>

                            <div class="column">
                                <h4>Experimental.</h4>
                                <p>I should at least try and experiment with this website – is basic HTML okay to log posts with? Do I need a content management system (like netlify CMS)? In a coffee shop I tried out HUGO, with GitHub, a Hugo theme, and Netlify CMS. The result was a very boring looking website which is easy for me to update. That’s completely the wrong way round in my opinion – if I do have to choose, it should be hard for me to update but beautiful for you to read!</p>
                            </div>

                            <div class="column">
                                <h4>Blog From Anywhere.</h4>
                                <p>As any parent in my position (with young children) will know, time is of the essence always and having any kind of spare time is impossible. Anything goes – this entire page you are reading has been dictated while I was getting ready, then edited over breakfast, so if I can try and cram in anything in my busy life to get something up on the site, then it’s gonna be worth trying!</p>
                            </div>
                        </div>

                    </div> <!-- end s-content__primary -->

                </section>

            </div> <!-- end column -->
        </div> <!-- end row -->
    </section> <!-- end s-content -->


    <!-- footer
    ================================================== -->
    <footer class="s-footer">

        <div class="s-footer__main">

            <div class="row">

                <div class="column large-4 medium-6 tab-12 s-footer__info">

                    <h5>About K8Simon</h5>

                    <p>
                    All about kubernetes. This site uses the amazing Azure Static Web apps (free hosting, free SSL), an adapted HTML5 theme and Microsoft's Blazor Web Assembly. Pull up a chair, hang out a while.
                    </p>

                </div> <!-- end s-footer__info -->

                <div class="column large-2 medium-3 tab-6 s-footer__site-links">

                    <h5>Site Links</h5>

                    <ul>
                        <li><a href="#0">About Us</a></li>
                        <li><a href="#0">Blog</a></li>
                        <li><a href="#0">FAQ</a></li>
                        <li><a href="#0">Terms</a></li>
                        <li><a href="#0">Privacy Policy</a></li>
                    </ul>

                </div> <!-- end s-footer__site-links -->  

                <div class="column large-2 medium-3 tab-6 s-footer__social-links">

                    <h5>Social</h5>

                    <ul>
                        <li><a href="#0">Twitter</a></li>
                        <li><a href="#0">Facebook</a></li>
                        <li><a href="#0">Dribbble</a></li>
                        <li><a href="#0">Pinterest</a></li>
                        <li><a href="#0">Instagram</a></li>
                    </ul>

                </div> <!-- end s-footer__social links --> 

                <div class="column large-4 medium-12 s-footer__subscribe">

                    <h5>Subscribe</h5>

                    <p>Keep yourself updated. Subscribe to our newsletter.</p>

                    <div class="subscribe-form">
                
                        <form id="mc-form" class="group" novalidate="true">

                            <input type="email" value="" name="dEmail" class="email" id="mc-email" placeholder="Type &amp; press enter" required=""> 
                
                            <input type="submit" name="subscribe" >
                
                            <label for="mc-email" class="subscribe-message"></label>
                
                        </form>

                    </div>

                </div> <!-- end s-footer__subscribe -->

            </div> <!-- end row -->

        </div> <!-- end s-footer__main -->

        <div class="s-footer__bottom">
            <div class="row">
                <div class="column">
                    <div class="ss-copyright">
                        <span>© Simon C 2022</span> 
                        <span>Design by <a href="https://www.styleshout.com/">StyleShout</a></span>		         	
                    </div> <!-- end ss-copyright -->
                </div>
            </div> 

            <div class="ss-go-top">
                <a class="smoothscroll" title="Back to Top" href="#top">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M6 4h12v2H6zm5 10v6h2v-6h5l-6-6-6 6z"/></svg>
                </a>
            </div> <!-- end ss-go-top -->
        </div> <!-- end s-footer__bottom -->

   </footer>   
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'About us'
  }
}
</script>
