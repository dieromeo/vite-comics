<script>
import Social from './Social.vue';
import SignupButton from './SignupButton.vue';
export default {
    name: 'BottomBar',
    components: {
        Social,
        SignupButton
    }
}
</script>
<template>
    <div class="bottom-bar">
        <div class="container">
            <SignupButton></SignupButton>
            <Social></Social>
        </div>
    </div>
</template>

<style lang="scss">
@use '../style/main.scss' as *;

.bottom-bar {
    background-color: $footer-bg;
}
</style>