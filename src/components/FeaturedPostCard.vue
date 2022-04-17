<template>
<div class="featured-post-slide">
    <div class="f-slide">
        <div class="f-slide__background" :style="image"></div>
        <div class="f-slide__overlay"></div>

        <div class="f-slide__content">
            <ul class="f-slide__meta">
                <li>{{ date }}</li> 
                <li><g-link :to="link">{{ title }}</g-link></li>
            </ul>	

            <h1 class="f-slide__title"><g-link :to="link">{{ description }}</g-link></h1> 
        </div>

    </div> <!-- f-slide -->
</div>
</template>


<script>
export default {
    name: 'FeaturedPostCard',
    props: ['image', 'date', 'title', 'description', 'link']
}
</script>