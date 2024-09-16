<script>
export default {
    data() {
        return {
            
        }
    }
}
</script>

<template>
    <footer>
        <div class="container">
            <div class="cta-footer">
                <div class="digital-comics">
                    <img src="../../assets/img (5)/img/buy-comics-digital-comics.png" alt="digital comics">
                    <p>digital comics</p>
                </div>
                <div class="dc-merchandise">
                    <img src="../../assets/img (5)/img/buy-comics-merchandise.png" alt="dc merchandise">
                    <p>dc merchandise</p>
                </div>
                <div class="subscription">
                    <img src="../../assets/img (5)/img/buy-comics-subscriptions.png" alt="digital comics">
                    <p>subscription</p>
                </div>
                <div class="comic-shop-locator">
                    <img src="../../assets/img (5)/img/buy-comics-shop-locator.png" alt="digital comics">
                    <p>comic shop locator</p>
                </div>
                <div class="dc-power-visa">
                    <img src="../../assets/img (5)/img/buy-dc-power-visa.svg" alt="digital comics">
                    <p>dc power visa</p>
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped>
    footer {
        background-color: #0282F9;
        height: 150px;
    }

    .cta-footer {
        display: flex;
        justify-content: space-around;
        gap: 20px;
        align-items: center;
        height: 150px;

        img {
            height: 50px;
        }

        p {
            color: white;
            margin: 0;
            text-transform: uppercase;
        }
    }

    .cta-footer > * {
        display: flex;
        align-items: center;
        justify-content: space-around;
        gap: 10px;
    }
</style>