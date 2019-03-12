<template>
    <div class="input">
        <input :type="input.type" :placeholder="input.type">
    </div>
</template>

<script>
export default {
    props: {
        input: {
            type: Object,
            required: true,
        }
    }
}
</script>

<style lang="scss" scoped>

</style>
