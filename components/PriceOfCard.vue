<style lang="scss" scoped>
.card-price {
  padding: 8px 14px;
  border-radius: 0px 0px 20px 20px;
  @include space-between-flex;
  &__text {
    color: $white;
    font-weight: 700;
    font-size: 35px;
  }
  &__icons {
    display: flex;
    align-items: center;
    gap: 10px;
    padding: 6px 8px;
    border-radius: 8px;
    background-color: $white;
  }
}
</style>
<template>
  <div :style="{ background: color }" class="card-price">
    <span class="card-price__text">{{ price }}</span>
    <div class="card-price__icons">
      <svg
        width="25"
        height="24"
        viewBox="0 0 25 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M1.69336 6.6123H23.3457L22.1428 22.8516H2.89627L1.69336 6.6123Z"
          :stroke="color"
          stroke-width="2"
          stroke-linejoin="round"
        />
        <path
          d="M7.70801 9.01812V1.19922H17.3313V9.01812"
          :stroke="color"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M7.70801 18.04H17.3313"
          :stroke="color"
          stroke-width="2"
          stroke-linecap="round"
        />
      </svg>
      <svg
        width="20"
        height="20"
        viewBox="0 0 20 20"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M9.7666 1.60352V18.4473"
          :stroke="color"
          stroke-width="2"
          stroke-linecap="round"
        />
        <path
          d="M18.1895 10.0254L1.3457 10.0254"
          :stroke="color"
          stroke-width="2"
          stroke-linecap="round"
        />
      </svg>
    </div>
  </div>
</template>

<script setup>
defineProps({
  price: String,
  color: String,
});
</script>
