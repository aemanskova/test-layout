<template>
  <div class="card">
    <HeadingOfCard color="#ffca00" heading="LITE"></HeadingOfCard>
    <UltraCard
      zIndex="100"
      color="#81b42e"
      small
      left="7%"
      :spans="['ONLINE STORE APP', 'CRM SYSTEM']"
    ></UltraCard>
    <UltraCard
      zIndex="110"
      monochrome
      small
      left="70%"
      :spans="['LOYALTY SYSTEM']"
    ></UltraCard>
    <PriceOfCard price="$75k" color="#ffca00"></PriceOfCard>
  </div>
</template>
<style lang="scss" scoped>
.card {
  width: 240px;
}
</style>
