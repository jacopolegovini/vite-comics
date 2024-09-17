<script>
export default {
    data() {
        return {
            
        }
    }
}
</script>

<template>
    <div class="top-main-img">
        <div class="current-series">
            Current Series
        </div>
    </div>
</template>

<style scoped>
    .top-main-img {
        background-image: url(../../assets/img/img/jumbotron.jpg);
        height: 30%;
        position: relative;
    }

    .current-series {
        text-transform: uppercase;
        background-color: #0282F9;
        color: white;
        padding: 5px 8px;
        display: inline;
        text-align: center;
        font-weight: 500;
        position: absolute;
        bottom: -15px;
        left: 300px;
    }
</style>