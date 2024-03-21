<style lang="scss" scoped>
.card-heading {
  padding: 30px 32px;
  border-radius: 20px 20px 0px 0px;
  &__text {
    color: $white;
    font-weight: 700;
    font-size: 50px;
    padding-right: 0;
    @include center-flex;
  }
}
</style>
<template>
  <div :style="{ background: color }" class="card-heading">
    <span class="card-heading__text">{{ heading }}</span>
  </div>
</template>

<script setup>
defineProps({
  heading: String,
  color: String,
});
</script>
