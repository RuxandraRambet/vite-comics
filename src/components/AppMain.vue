<script>
import MainContentComponent from './MainContentComponent.vue';
import MainIconsComponentVue from './MainIconsComponent.vue';
export default {
    name: 'AppMain',
    components: {
        MainContentComponent,
        MainIconsComponentVue,
    }
}
</script>

<template>
    <main>
        <MainContentComponent />
        <MainIconsComponentVue />
    </main>
 
</template>

<style lang="scss">

</style>