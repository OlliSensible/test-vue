<template>
  <ContainerForItem>
    <slot name="title"></slot>
    <div class="apartments-list">
      <template v-for="apartment in items">
        <slot name="apartment" v-bind:apartment="apartment"></slot>
      </template>
    </div>
  </ContainerForItem>
</template>

<script>
import ContainerForItem from '../shared/ContainerForItem'

export default {
  name: 'ApartmentsList',
  components: {
    ContainerForItem,
  },
  props: {
    items: {
      type: Array,
      default: () => [],
    },
  },
}
</script>

<style lang="scss" scoped>
.apartments-list {
  display: flex;
  flex-wrap: wrap;
  margin-left: -15px;
  margin-right: -15px;
}
</style>