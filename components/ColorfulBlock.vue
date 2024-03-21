<template>
  <div :style="{ background: color, zIndex: zIndex }" class="colorful-block">
    <div class="colorful-block__text">
      <span class="colorful-block__span">{{ span }}</span>
      <span class="colorful-block__span">{{ price }}</span>
    </div>

    <div
      :style="{ background: color, left: left }"
      class="colorful-block__part"
    >
      <svg
        class="colorful-block__arrow"
        width="65"
        height="32"
        viewBox="0 0 65 32"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M62.6699 2.64307L32.6699 28.6431L2.66992 2.64307"
          stroke="white"
          stroke-width="4"
          stroke-linecap="round"
        />
      </svg>
    </div>
  </div>
</template>
<script setup>
defineProps({
  span: String,
  left: String,
  color: String,
  price: String,
  zIndex: String,
});
</script>
<style lang="scss" scoped>
.colorful-block {
  max-height: 150px;
  padding: 15px 60px;
  position: relative;
  &__text {
    color: $white;
    @include space-between-flex;
  }
  &__span {
    font-weight: 700;
    font-size: 22px;
  }
  &__part {
    background-color: $white;
    position: absolute;
    bottom: -72%;
    width: 80px;
    height: 40px;
    border-radius: 0 0 24px 24px;
  }
  &__arrow {
    position: absolute;
    margin-left: auto;
    margin-right: auto;
    left: 0;
    right: 0;
    top: 20%;
    max-width: 30px;
  }
}
@media (min-width: 768px) {
  .colorful-block {
    padding: 20px 80px;
    &__span {
      font-size: 32px;
    }
    &__part {
      bottom: -84%;
      width: 120px;
      height: 70px;
      border-radius: 0 0 32px 32px;
    }
    &__arrow {
      max-width: 50px;
    }
  }
}
@media (min-width: 1440px) {
  .colorful-block {
    padding: 25px 100px;
    &__span {
      font-size: 64px;
    }
    &__part {
      bottom: -70%;
      width: 165px;
      height: 87px;
      border-radius: 0 0 40px 40px;
    }
    &__arrow {
      max-width: 60px;
    }
  }
}
</style>
