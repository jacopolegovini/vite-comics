<script>
export default {
    data() {
        return {
            flag: false,
            currentIndex: null,
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
            ],
            sandwichMenus: [
                'lorem ipsum',
                'lorem ipsum',
                'lorem ipsum',
                'lorem ipsum',
                'lorem ipsum',
                'lorem ipsum',
                'lorem ipsum',
            ]            
        }
    },
    methods: {
            changeValueNavbar(index) {
                return this.currentIndex = index;
            },
            
            disappearMenu(){
                return this.currentIndex = null;
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
                    <li v-for="(list, index) in menu" :key="index" @click="changeValueNavbar(index)">
                        <div :class="currentIndex === index ? 'highlight-navbar' : ''">{{ list }}</div>
                    </li>
                </ul>
            </div>
        </div>
        <div class="sandwich-menu" v-if="currentIndex !== null" :class="currentIndex">
            <div>
                <div class="container" v-for="(list, index) in sandwichMenus" :key="index" @click="disappearMenu">
                    {{ list }}
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped>
    .highlight-navbar {
        border-bottom: 2px solid #0282F9;
        color: #0282F9;
        height: 149.5px;
    }

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
            cursor: pointer;
        }

    }

    /* ul li:nth-child(2) {
        border-bottom: 2px solid #0282F9;
        color: #0282F9;
    } */

    .sandwich-menu {
        position: relative;
        z-index: 1;
        color: black;
        background-color: white;
        height: 270px;
    }

</style>
