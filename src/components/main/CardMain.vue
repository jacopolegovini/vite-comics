<script>
export default {
    data() {
        return {
            
        }
    },
    props: {
        comic: {
            thumb: String,
            price: Number,
            series: String,
            type: String
        }
    }
}
</script>

<template>
    <main>
        <h1>{{comic.price}}</h1>
    </main>
</template>

<style scoped>

</style>