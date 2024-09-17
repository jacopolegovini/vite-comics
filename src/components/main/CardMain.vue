<script>
export default {
    data() {
        return {
            
        }
    },
    props: {
        comic: {
            thumb: {
                type: String,
                required: true
            },
            price: {
                type: Number,
                required: false
            },
            series: {
                type: String,
                required: true
            },
            type: {
                type: String,
                required: false
            }
        }
    },
    methods: {
        getImagePath(imgPath) {
            return new URL (imgPath, import.meta.url).href;
        }
    }
}
</script>

<template>
    <main>
        <div class="comic-card">
            <div class="card-img">
                <img :src="comic.thumb" :alt="comic.series">
            </div>
        </div>
    </main>
</template>

<style scoped>
    main {
        flex-basis: calc((100% / 6) - (100px / 3));
    }
    
    .card-img {
        height: 200px;
    }

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: 0 0;
    }
</style>