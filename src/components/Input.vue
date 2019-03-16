<template>
    <div class="input">
        <input :type="input.type" :placeholder="input.type">
        <i :class="[classes.icon, input.icon]"></i>
    </div>
</template>

<script>
export default {
    data() {
      return{
          classes: {
              icon: 'far',
          }
      }
    },
    props: {
        input: {
            type: Object,
            required: true,
        }
    }
}
</script>

<style lang="scss" scoped>
    .input {
        position: relative;
        width: 100%;
        display: flex;
        justify-content: center;

        & > input {
            width: 100%;
            padding: 1.5rem 0 1rem 0;
            padding-left: 2.5rem;
            border: none;
            border-bottom: 1px solid #bbb;
            outline: none;
            background: none;
            color: #fff;
            transition: all .3s;

            &::placeholder {
                font-size: 1.5rem;
                color: #CECECE;
                text-transform: capitalize;
                transition: all .3s;
            }

            &:focus {
                border-bottom: 1px solid #fff;
            }

            &:focus::placeholder {
                transform: translateX(3rem);
                opacity: 0
            }
        }

        & > input:focus + i {
            color: #fff;
        }

        & > i {
            position: absolute;
            top: 50%;
            left: 1rem;
            transform: translate(-50%, -50%);
            font-size: 1.5rem;
            font-weight: bold;
            color: #aaa;
            transition: color .3s;
        }

        &:not(:last-child) {
            margin-bottom: 2rem;
        }
    }
</style>
