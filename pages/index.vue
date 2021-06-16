<template>
    <div class="hero">
        <h2>Selamat Datang</h2><br>
        <p>NuxtBlog menambah pengetahuan seputar dunia blogging</p>
        <br>
        <nuxt-link to="/posts"><button class="button--green">Baca</button></nuxt-link>
    </div>
</template>

<style scoped>
    .hero {
        display: flex;
        flex-flow: column;
        margin: 10px;
        justify-content: center;
        align-items: center;
        margin-top: 50px;
    }
</style>