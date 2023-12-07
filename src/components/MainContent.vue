<script>
export default {
    name: 'ContentMain',
    data() {
        return {
            futureContent: '--> Content goes here <--'
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="content-title">
            <h2>{{ futureContent }}</h2>
        </div>
    </div>
</template>

<style lang="scss">
@use '../style/main.scss' as *;

.content-title {
    color: $titles;
    padding: 45px 0;
}
</style>