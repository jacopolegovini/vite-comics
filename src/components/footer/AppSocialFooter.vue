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
        <div class="container social-footer">
            <div class="sign-up">
                <p>SIGN-UP NOW!</p>
            </div>
            <div class="social-icon">
                <p>FOLLOW ME</p>
                <img src="../../assets/img/img/footer-facebook.png" alt="Facebook">
                <img src="../../assets/img/img/footer-twitter.png" alt="Twitter">
                <img src="../../assets/img/img/footer-youtube.png" alt="Youtube">
                <img src="../../assets/img/img/footer-pinterest.png" alt="Pinterest">
                <img src="../../assets/img/img/footer-periscope.png" alt="Periscope">
            </div>
        </div>
    </footer>
</template>

<style scoped>
    footer {
        background-color: #303030;
    }
    .social-footer {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 30px;
    }

    .social-icon {
        display: flex;
        justify-content: space-around;
        align-items: center;
        gap: 10px;
    }

    .sign-up p {
        color: white;
        border: 2px solid #0282F9;
        margin: 0;
        padding: 5px 8px;
    }

    .social-icon p {
        color: #0282F9;
        margin: 0;
        font-weight: bold;
        margin-right: 10px;
    }
</style>