<template>
    <button>
        <slot></slot>
    </button>
</template>

<script>
    export default {
        name: 'ButtonFirst',
        props: {
            type: String
        }
    }
</script>

<style lang="scss" scoped>


</style>