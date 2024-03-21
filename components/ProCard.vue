<template>
  <div class="card">
    <HeadingOfCard color="#ff4e68" heading="PRO"></HeadingOfCard>
    <UltraCard
      zIndex="100"
      color="#81b42e"
      small
      left="7%"
      :spans="['ONLINE STORE APP', 'CRM SYSTEM']"
    ></UltraCard>
    <UltraCard
      zIndex="110"
      color="#ffca00"
      small
      left="70%"
      :spans="['LOYALTY SYSTEM']"
    ></UltraCard>
    <UltraCard
      zIndex="120"
      color="#ff8f28"
      small
      left="70%"
      :spans="['SOCIAL MEDIA', 'NEWS FEED', 'MULTILINGUAL']"
    ></UltraCard>
    <UltraCard
      zIndex="130"
      monochrome
      small
      left="74%"
      :spans="['BONUSES FOR FRIENDS']"
    ></UltraCard>
    <PriceOfCard price="$150k" color="#ff4e68"></PriceOfCard>
  </div>
</template>
<style lang="scss" scoped>
.card {
  width: 240px;
}
</style>
