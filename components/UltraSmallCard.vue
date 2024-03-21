<template>
  <div class="card">
    <HeadingOfCard color="#8c35e3" heading="PRO"></HeadingOfCard>
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
      color="#ff4e68"
      small
      left="75%"
      :spans="['BONUSES FOR FRIENDS']"
    ></UltraCard>
    <UltraCard
      zIndex="140"
      monochrome
      small
      smallGap
      left="74%"
      :spans="['CUSTOMIZABLE', 'CALENDAR']"
    ></UltraCard>
    <UltraCard
      zIndex="150"
      monochrome
      small
      left="60%"
      :spans="['BUSINESS VERSION']"
    ></UltraCard>
    <UltraCard
      zIndex="160"
      monochrome
      small
      smallGap
      left="70.2%"
      :spans="['YOUR PAYMENT', 'SYSTEM']"
    ></UltraCard>
    <UltraCard
      zIndex="170"
      monochrome
      small
      left="60%"
      :spans="['GIFTS FOR CUSTOMERS']"
    ></UltraCard>
    <UltraCard
      zIndex="180"
      monochrome
      small
      smallGap
      left="74%"
      :spans="['NEED FEED']"
    ></UltraCard>
    <PriceOfCard price="$150k" color="#8c35e3"></PriceOfCard>
  </div>
</template>
<style lang="scss" scoped>
.card {
  width: 240px;
}
</style>
