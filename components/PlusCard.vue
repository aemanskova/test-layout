<template>
  <div class="card">
    <HeadingOfCard color="#ff8f28" heading="PLUS"></HeadingOfCard>
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
      monochrome
      small
      left="70%"
      :spans="['SOCIAL MEDIA']"
    ></UltraCard>
    <UltraCard
      zIndex="130"
      monochrome
      small
      left="74%"
      :spans="['NEWS FEED']"
    ></UltraCard>
    <UltraCard
      zIndex="140"
      monochrome
      small
      left="60%"
      :spans="['MULTILINGUAL']"
    ></UltraCard>
    <PriceOfCard price="$150k" color="#ff8f28"></PriceOfCard>
  </div>
</template>
<style lang="scss" scoped>
.card {
  width: 240px;
}
</style>
