<script>
export default {
    data() {
        return {
            menu: [
                'Characters',
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Collectibles',
                'Videos',
                'Fans',
                'News',
                'Shop'
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="header-flex">
            <div class="img-header">
                <img src="../assets/img (5)/img/dc-logo.png" alt="logo DC">
            </div>
            <div class="navbar-header">
                <ul class="navbar-header-flex d-flex">
                    <li v-for="list in menu">
                        {{ list }}
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style scoped>
    .header-flex {
        padding: 20px;
        display: flex;
        justify-content: center;
        align-items: center;

        .img-header {
            flex-basis: 50%;
            text-align: center;
        }

        .navbar-header-flex {
            gap: 15px;
            text-align: center;
        }
    }


</style>
