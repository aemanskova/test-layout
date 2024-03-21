<template>
  <span :style="{ color: color }" class="price">{{ price }}</span>
</template>
<script setup>
defineProps({
  price: String,
  color: String,
});
</script>
<style lang="scss" scoped>
.price {
  font-size: 18px;
  font-weight: 700;
}
@media (min-width: 790px) {
  .price {
    font-size: 24px;
  }
}
@media (min-width: 790px) {
  .price {
    font-size: 64px;
  }
}
</style>
