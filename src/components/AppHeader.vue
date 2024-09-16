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
        <div class="container header-flex">
            <div class="img-header">
                <img src="../assets/img/img/dc-logo.png" alt="logo DC">
            </div>
            <div class="navbar-header">
                <ul class="navbar-header-flex">
                    <li v-for="list in menu">
                        {{ list }}
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style scoped>
    header {
        height: 150px;
    }

    .header-flex {
        height: 100%;
        padding: 0;
        display: flex;
        justify-content: space-between;
        align-items: center;

        .img-header {
            flex-basis: 40%;
        }

        .navbar-header {
            height: 100%;
        }

        .navbar-header-flex {
            gap: 15px;
            font-weight: bold;
            color: gray;
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100%;
        }

        ul {
            margin: 0;
        }

        li {
            height: 100%;
            text-transform: uppercase;
            line-height: 150px;
        }

    }

    ul li:nth-child(2) {
        border-bottom: 2px solid #0282F9;
        color: #0282F9;
    }


</style>
