<style lang="scss" scoped>
.text {
  color: $black;
  @include flex-column;
  gap: 16px;
  max-width: 560px;
  &__heading {
    font-size: 32px;
    font-weight: 700;
  }
  &__text {
    font-size: 24px;
  }
}
</style>
<template>
  <div class="text">
    <span class="text__heading">{{ heading }}</span>
    <p class="text__content">{{ text }}</p>
  </div>
</template>

<script setup>
defineProps({
  heading: String,
  text: String,
});
</script>
