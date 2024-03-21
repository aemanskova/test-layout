<template>
  <div class="cards">
    <UltraCard
      zIndex="80"
      color="#81b42e"
      left="5%"
      :spans="['ONLINE STORE APP', 'CRM SYSTEM']"
    ></UltraCard>
    <UltraCard
      zIndex="100"
      color="#ffca00"
      :spans="['LOYALTY SYSTEM']"
    ></UltraCard>
    <UltraCard
      zIndex="200"
      left="5%"
      color="#ff8f28"
      :spans="['SOCIAL MEDIA', 'NEWS FEED', 'MULTILINGUAL']"
    ></UltraCard>
    <UltraCard
      zIndex="300"
      color="#ff4e68"
      smallGap
      :spans="['BONUSES', 'FOR FRIENDS']"
    ></UltraCard>
  </div>
</template>
<style lang="scss" scoped>
.cards {
  @include flex-column;
  max-width: max-content;
}
</style>
