<script>
export default {
    name: 'BlueButton'
}
</script>

<template>
    <button> Load more </button>
</template>

<style lang="scss" scoped>
@use '../style/main.scss' as *;

button {
    all: unset;
    background-color: $button-br;
    padding: 10px;
    color: $titles;
    padding: 10px 60px;
    cursor: pointer;
    text-transform: uppercase;
    font-size: 14;
    font-weight: bold;
    margin-bottom: 20px;

}
</style>