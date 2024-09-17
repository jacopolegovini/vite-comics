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
    <div class="card-main">
        <div class="comic-card">
            <div class="card-img">
                <img :src="comic.thumb" :alt="comic.series">
                <p>{{ comic.series }}</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
    .card-main {
        flex-basis: calc((100% / 6) - (100px / 3));
        padding: 15px 0;
    }

    p {
        margin: 0;
        color: white;
        text-transform: uppercase;
        font-size: 0.9rem;
        font-weight: bold;
    }

    .card-img {
        height: 200px;
    }

    img {
        margin-bottom: 5px;
    }

    img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: 0 0;
    }
</style>