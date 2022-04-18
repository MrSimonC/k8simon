<template>
    <article class="brick entry format-quote animate-this" >

        <div class="entry__thumb">
            <blockquote>
                <p>{{ quote }}</p>

                <cite>{{ author }}</cite>
                <cite>{{ authortitle }}</cite>
            </blockquote>
        </div>

    </article>
</template>

<script>
export default {
    name: 'CardQuote',
    props: ['quote', 'author', 'authortitle']
}
</script>