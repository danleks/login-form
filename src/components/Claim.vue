<template>
    <header class="claim">
        <h1>Hello there!</h1>
        <p>We are so excited to meet you!</p>
    </header>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .claim {
        flex: 2;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;

        & > h1 {
            color: #fff;
            font-size: 3.5rem;
            font-weight: 100;
            line-height: 1.5;
        }

        & > p {
            font-size: 1.7rem;
            color: #7C7C7C;
        }
    }

</style>
