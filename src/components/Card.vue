<script>
export default {
    name: 'Card',
    props: {
        image: String,
        title: String
    }
}
</script>

<template>
    <div class="card">
        <div class="card-image">
            <img :src="image" alt="">
        </div>
        <div class="card-title">
            <h4>{{ title.toUpperCase() }}</h4>
        </div>
    </div>
</template>

<style>
.card-image img {
    width: 100%;
    display: block;
}
</style>