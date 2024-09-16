<script>
export default {
    data() {
        return {
            dcLists: {
                dcComics: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"],
                dc: ["Terms Of Use", "Privacy policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"],
                sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
                shop: ["Shop DC", "Shop DC Collectibles"]
            }
        }
    }
}
</script>

<template>
    <footer>
        <div class="container list-footer">
            <ul>
                <h5>DC COMICS</h5>
                <li v-for="element in dcLists.dcComics">{{element}}</li>
                <h5 class="mt-3">SHOP</h5>
                <li v-for="element in dcLists.shop">{{ element }}</li>
            </ul>
            <ul>
                <h5>DC</h5>
                <li v-for="element in dcLists.dc">{{element}}</li>
            </ul>
            <ul>
                <h5>SITES</h5>
                <li v-for="element in dcLists.sites">{{element}}</li>
            </ul>
        </div>
    </footer>
</template>

<style scoped>
    footer {
        background-image: url(../../assets/img/img/footer-bg.jpg);
        padding: 30px;
    }

    .list-footer {
        display: flex;
    }

    ul {
        display: flex;
        flex-direction: column;
        color: white;
        
        li {
            opacity: 0.5;
        }
    }

    h5 {
        color: white;
    }
</style>