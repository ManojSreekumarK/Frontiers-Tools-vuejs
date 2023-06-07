<template>
  <div>
    <img src="@/assets/icons/businessworkflow.svg" />
    <span>Article {{ pid }}</span>
    <h2>businessworkflow</h2>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Cupiditate, similique quidem! Ab?
    </p>
  </div>
</template>

<script setup lang="ts">
import { defineProps, computed } from 'vue'
import { useProductStore } from '@/stores/ProductStore'
const ProductStore = useProductStore()
const props = defineProps(['pid'])
const displayedProduct = computed(() => {
  ProductStore.getProductsById(props.pid)
})
console.log(displayedProduct)
</script>
<style lang="scss" scoped>
div {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
