<template>
<article class="brick entry format-video animate-this">
    
        <div class="entry__thumb">
            <g-link :to="link" class="thumb-link">
                <g-image :src="image" :alt="title"></g-image>
            </g-link>
        </div> <!-- end entry__thumb -->

        <div class="entry__text">
            <div class="entry__header">

                <!-- <div class="entry__meta">
                    <span class="entry__cat-links">
                        <a href="#">Design</a> 
                        <a href="#">Photography</a>
                    </span>
                </div> -->

                <h1 class="entry__title"><g-link :to="link">{{ title }}</g-link></h1>
                
            </div>
            <div class="entry__excerpt">
                <p>
                    {{ description }}
                </p>
            </div>
        </div> <!-- end entry__text -->

    </article>
</template>

<script>
export default {
    name: 'CardVideo',
    props: ['image', 'title', 'description', 'link']
}
</script>