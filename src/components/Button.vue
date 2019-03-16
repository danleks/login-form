<template>
    <div class="authenticate">
        <button class="authenticate__button">Authenticate</button>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .authenticate {
        flex: 1;
        display: flex;
        align-items: center;
        width: 90%;

        @media(min-width: 768px) {
            flex: 1;
        }

        &__button {
            width: 100%;
            padding: 1.5rem;
            border: none;
            font-size: 1.8rem;
            color: #fff;
            background-color: #CE6060;

            @media(min-width: 768px) {
                font-size: 2.5rem;
            }
        }
    }
</style>
