<template>
     <video autoplay muted loop class="video">
        <source src="../assets/bg.mp4" type="video/mp4">
    </video>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .video {
        position: fixed;
        bottom: 0;
        min-width: 100%;
        min-height: 100%;
        z-index: -1;
    }
</style>
