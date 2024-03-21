<template>
  <div class="cards">
    <UltraCard
      zIndex="70"
      monochrome
      smallGap
      :spans="['CUSTOMIZABLE', 'CALENDAR']"
    ></UltraCard>
    <UltraCard
      zIndex="100"
      monochrome
      :spans="['BUSINESS VERSION']"
    ></UltraCard>
    <UltraCard
      zIndex="150"
      monochrome
      smallGap
      :spans="['YOUR PAYMENT', 'SYSTEM']"
    ></UltraCard>
    <UltraCard
      zIndex="200"
      monochrome
      smallGap
      :spans="['GIFTS', 'FOR CUSTOMERS']"
    ></UltraCard>
    <UltraCard
      zIndex="250"
      monochrome
      smallGap
      :spans="['YOUR', 'STICKERS` PACK']"
    ></UltraCard>
  </div>
</template>
<style lang="scss" scoped>
.cards {
  @include flex-column;
  max-width: max-content;
}
</style>
