<template>
    <div class="authenticate">
        <button type="submit" class="authenticate__button">Authenticate</button>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .authenticate {
        display: flex;
        align-items: flex-start;
        width: 100%;

        @media(min-width: 768px) {
           //
        }

        &__button {
            width: 100%;
            padding: 1.5rem;
            border: none;
            font-size: 1.8rem;
            color: #fff;
            background-color: #CE6060;
            cursor: pointer;

            @media(min-width: 768px) {
                font-size: 2.5rem;
            }
        }
    }
</style>
