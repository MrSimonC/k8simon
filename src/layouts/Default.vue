<template>
  <div class="layout">
    <!-- header
    ================================================== -->
    <header class="s-header" id='top'>

        <div class="row s-header__content">

            <div class="s-header__logo">
                    <g-link to="/"><g-image src="~/../static/images/logo.svg" alt="Homepage" /></g-link>
                </a>
            </div>

            <nav class="s-header__nav-wrap">

                <h2 class="s-header__nav-heading h6">Site Navigation</h2>

                <ul class="s-header__nav">
                    <!-- <li class="current"><a href="index.html" title="">Home</a></li> -->
                    <li><g-link to="/">Home</g-link></li>
                    <li><g-link to="/about/">About us</g-link></li>
                </ul> <!-- end header__nav -->

                <a href="#0" title="Close Menu" class="s-header__overlay-close close-mobile-menu">Close</a>

            </nav> <!-- end header__nav-wrap -->
                   
            <a class="s-header__toggle-menu" href="#0" title="Menu"><span>Menu</span></a>
            
            <div class="s-header__search">
                    
                <form role="search" method="get" class="s-header__search-form" action="#">
                    <label>
                        <span class="hide-content">Search for:</span>
                        <input type="search" class="s-header__search-field" placeholder="Type Your Keywords" value="" name="s" title="Search for:" autocomplete="off">
                    </label>
                    <input type="submit" class="s-header__search-submit" value="Search">
                </form>

                <a href="#0" title="Close Search" class="s-header__overlay-close">Close</a>

            </div> <!-- end search wrap -->	

            <a class="s-header__search-trigger" href="#">
                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M10 18a7.952 7.952 0 004.897-1.688l4.396 4.396 1.414-1.414-4.396-4.396A7.952 7.952 0 0018 10c0-4.411-3.589-8-8-8s-8 3.589-8 8 3.589 8 8 8zm0-14c3.309 0 6 2.691 6 6s-2.691 6-6 6-6-2.691-6-6 2.691-6 6-6z"></path></svg>
            </a>

        </div> <!-- end s-header__content -->

    </header> <!-- end header -->
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>
<!-- 
<style>
body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}

.layout {
  max-width: 760px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}

.nav__link {
  margin-left: 20px;
}
</style> -->
