<template>
    <button v-on= '$listeners' v-bind:type="type" class="btn btn--outlined">
        <slot></slot>
    </button>
</template>

<script>
    export default {
        name: 'ButtonFirst',
        props: {
            type: {
                type: String,
                default: 'button',
                required: true
            }
        }
    }
</script>

<style lang="scss" scoped>
    .btn {
        display: inline-block;
        background: #000;
        color: #fff;
        border: none;
        padding: 10px 20px;
        margin: 5px;
        border-radius: 5px;
        cursor: pointer;
        text-decoration: none;
        font-size: 15px;
        font-family: inherit;
    }
</style>