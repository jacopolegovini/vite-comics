<script>
import AppCtaFooter from './footer/AppCtaFooter.vue';
import AppListFooter from './footer/AppListFooter.vue';
import AppSocialFooter from './footer/AppSocialFooter.vue';

export default {
    data() {
        return {
            
        }
    },
    components: {
        AppCtaFooter,
        AppListFooter,
        AppSocialFooter
    }
}
</script>

<template>
    <footer>
        <AppCtaFooter/>
        <AppListFooter/>
        <AppSocialFooter/>
    </footer>
</template>

<style scoped>

</style>
