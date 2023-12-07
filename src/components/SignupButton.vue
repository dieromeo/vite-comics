<script>
export default {
    name: 'SignupButton',
    data() {
        return {
            buttonContent: 'Sign-up now'
        }
    }
}
</script>

<template>
    <button>{{ buttonContent.toUpperCase() }}</button>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;

button {
    all: unset;
    color: white;
    padding: 15px;
    border: 2px solid $button-br;
    margin: 20px 0;
    font-size: 14px;
}
</style>