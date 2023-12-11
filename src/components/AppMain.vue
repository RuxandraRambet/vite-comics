<script>
import MainContentComponent from './MainContentComponent.vue';
import MainIconsComponent from './MainIconsComponent.vue';

export default {
    name: 'AppMain',
    components: {
        MainContentComponent,
        MainIconsComponent,
    }
}
</script>

<template>
    <main>
        <MainContentComponent />
        <MainIconsComponent />
    </main>
 
</template>

<style lang="scss">

</style>