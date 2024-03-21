<template>
  <div
    :class="{
      card_monochrome: monochrome,
      card_small: small,
      card_small_with_border: small && monochrome,
    }"
    :style="{ background: color, zIndex: zIndex }"
    class="card"
  >
    <div
      :class="{
        card__part_monochrome: monochrome,
        card__part_small: small,
        card__part_small_with_border: small && monochrome,
      }"
      :style="{ background: color, left: left }"
      class="card__part"
    ></div>
    <div
      class="card__text"
      :class="{
        card__text_small_gap: smallGap,
        card__text_monochrome: monochrome,
        card__text_semibold: small,
      }"
    >
      <span class="card__span" v-for="span in spans" :key="span.idx">{{
        span
      }}</span>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.card {
  width: 200px;
  position: relative;
  padding: 40px 75px;
  border-radius: 15px;
  &_small {
    width: 200px !important;
    border-radius: 0px;
    padding: 25px 20px;
    &_with_border {
      width: 197px !important;
    }
  }
  &_monochrome {
    background-color: $white;
    border: 2px solid $black;
  }

  &__part {
    position: absolute;
    width: 90px;
    height: 50px;
    z-index: -1;
    border-radius: 15px 15px 0 0;
    bottom: 90%;
    left: 70%;
    &_small {
      height: 32px !important;
      width: 60px !important;
    }
    &_small_with_border {
      height: 24px !important;
      width: 60px !important;
    }
    &_monochrome {
      background-color: $white;
      height: 40px;
      bottom: 100%;
      @include part-border-style(2px, $black);
    }
  }
  &__text {
    @include flex-column;
    gap: 47px;
    font-size: 20px;
    font-weight: 700;
    color: $white;
    &_small_gap {
      gap: 5px;
    }
    &_monochrome {
      color: $black;
    }
    &_semibold {
      font-weight: 400;
      font-size: 16px;
    }
  }
}
</style>
<script setup>
defineProps({
  spans: Array,
  color: String,
  monochrome: Boolean,
  smallGap: Boolean,
  left: String,
  zIndex: String,
  small: Boolean,
});
</script>
