<template>
    <section class="posts">

        <Post
            thumbnail="https://disk.mediaindonesia.com/thumbs/1800x1200/news/2019/11/f33176d34d777c96ae913993e835ad18.jpg"
            title="Percobaan"
            previewText="Apakah kamu penasaran?"
            id="1"
        />
        
        <Post
            thumbnail="https://b.cloudcomputing.id/images/2c2027e0-233d-47ec-8366-a3ec69a85af0/iot-tren-min-min.jpg"
            title="Cloud Computing"
            previewText="Ini adalah bukti perkembangan bagus"
            id="2"
        />

    </section>
</template>

<script>
import Post from '@/components/Post';

export default {
    components: {
        Post
    }
}
</script>

<style scoped>
    .posts {
        display: flex;
        flex-flow: row wrap;
        justify-content: center;
        align-items: center;
    }
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
</style>


