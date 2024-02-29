<template>
    <div v-if="isVisible">
        <h1 v-show="false">Directives</h1>
        <ul>
            <template v-for="fruit in fruits">
                <li v-if="fruit === 'banana'" :key="fruit">
                    {{ fruit }}
                </li>
            </template>
        </ul>
    </div>
</template>

<script>
    export default {
    name: 'DirectivesTest',
        data () {
            return {
                isVisible: true,
                fruits: ['apple', 'banana', 'orange']
            }
        }
    }
</script>

<style lang="scss" scoped>

</style>