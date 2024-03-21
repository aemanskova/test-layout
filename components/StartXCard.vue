<template>
  <div class="card">
    <HeadingOfCard color="#81b42e" heading="STARTX"></HeadingOfCard>
    <UltraCard
      zIndex="100"
      monochrome
      small
      left="7%"
      :spans="['ONLINE STORE APP']"
    ></UltraCard>
    <UltraCard
      zIndex="110"
      monochrome
      small
      left="74%"
      :spans="['CRM SYSTEM']"
    ></UltraCard>
    <PriceOfCard price="$37.5k" color="#81b42e"></PriceOfCard>
  </div>
</template>
<style lang="scss" scoped>
.card {
  width: 240px;
}
</style>
