<script>
export default {
    name: 'Card',
    props: {
        image: String,
        title: String,
    }
}
</script>

<template>
    <div class="card" >
        <img :src="image" :alt="title">
        <h5>{{ title }}</h5>
    </div>
</template>

<style lang="scss"></style>