<template>
    <nuxt-link :to="'/posts/' + id">
        <article class="post">
            <div class="thumbnail" :style="{backgroundImage: 'url(' + thumbnail + ')'}"></div>
            <h1>{{ title }}</h1>
            <p>{{ previewText }}</p>
        </article>
    </nuxt-link>
    
</template>

<script>
export default {
    props: ['thumbnail','title','previewText','id']
}
</script>

<style scoped>
    .post {
        box-sizing: border-box;
        width: 300px;
        padding: 8px;
        border: 1px solid #ccc;
        box-shadow: 0 2px 2px #ddd;
        margin: 10px;
    }

    .post:hover {
        box-shadow: 4px 4px 4px #ccc;
    }

    .thumbnail {
     background-position: center;   
     background-size: cover;
     width: 100%;
     height: 200px;
    }

    a {
    text-decoration: none;
    color: black;
    }
</style>