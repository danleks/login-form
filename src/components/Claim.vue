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

        @media(min-width: 768px) {
            flex: 3;
        }

        @media(min-width: 1024px) {
            flex: 2;
        }

        & > h1 {
            color: #fff;
            font-size: 3.5rem;
            font-weight: 100;
            line-height: 1.5;

            @media(min-width: 768px) {
                font-size: 4.8rem;
            }

            @media(min-width: 1024px) {
                font-size: 4rem;
            }
        }

        & > p {
            font-size: 1.9rem;
            color: #7C7C7C;

            @media(min-width: 768px) {
                font-size: 4.2rem;
                font-weight: 100;
            }

            @media(min-width: 1024px) {
                font-size: 2rem;
            }
        }
    }

</style>
