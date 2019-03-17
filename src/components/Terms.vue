<template>
    <div class="terms">
        <p>By registering  I accept the</p>
        <p>
            <span>Terms of Service</span>
             and
            <span>Privacy Policy</span>
        </p>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .terms {
        flex: 1;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        font-size: 1.4rem;
        color: #7C7C7C;

        @media(min-width: 768px) {
            flex: 2;
            width: 100%;
            font-size: 2.4rem;
        }

        @media(min-width: 768px) {
            font-size: 2rem;
        }
    }

    span {
        color: #B1B2B3;
        cursor: pointer;
    }
</style>
