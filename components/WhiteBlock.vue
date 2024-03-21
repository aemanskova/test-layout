<template>
  <div class="colorful-block">
    <span class="colorful-block__span">PACKAGES</span>
    <div class="colorful-block__part"></div>
  </div>
</template>
<style lang="scss" scoped>
.colorful-block {
  background-color: $white;
  max-height: 150px;
  border-top: 4px solid $black;
  padding: 20px 60px;
  position: relative;
  &__span {
    font-weight: 700;
    font-size: 22px;
  }
  &__part {
    background-color: $white;
    position: absolute;
    top: -67%;
    left: 48%;
    width: 80px;
    height: 40px;
    @include part-border-style(4px, $black);
    border-radius: 24px 24px 0 0;
  }
}
@media (min-width: 768px) {
  .colorful-block {
    padding: 40px 80px;
    &__span {
      font-size: 32px;
    }
    &__part {
      top: -64%;
      width: 120px;
      height: 70px;
      border-radius: 32px 32px 0 0;
    }
  }
}
@media (min-width: 1440px) {
  .colorful-block {
    padding: 60px 100px;
    &__span {
      font-size: 64px;
    }
    &__part {
      top: -47%;
      width: 165px;
      height: 87px;
      border-radius: 40px 40px 0 0;
    }
  }
}
</style>
