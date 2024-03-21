<template>
  <div class="white-section">
    <img
      class="white-section__picture"
      src="../public/img/girl-white-section.png"
      alt=""
    />
    <BlackText
      class="white-section__text"
      heading="UPGRADING THE NEXT VERSION"
      text="You can start with any of the packages and upgrade over time once you need the added functionality"
    ></BlackText>
    <div class="white-section__strips">
      <div class="white-section__strip">
        <ColorfulStrip
          spanFrom="STARTX"
          spanTo="LIGHT"
          borderColor="#ffca00"
          bgColor1="#81b42e"
          bgColor2="#ffca00"
        >
          <template v-slot>
            <svg
              class="arrow"
              width="171"
              height="24"
              viewBox="0 0 171 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M2.76172 9.9126C1.65715 9.9126 0.761719 10.808 0.761719 11.9126C0.761719 13.0172 1.65715 13.9126 2.76172 13.9126V9.9126ZM170.988 11.9126L150.988 0.365592V23.4596L170.988 11.9126ZM2.76172 13.9126H152.988V9.9126H2.76172V13.9126Z"
                fill="white"
              />
            </svg> </template
        ></ColorfulStrip>
        <ColorfulPrice
          class="white-section__price"
          price="$52.5k"
          color="#ffca00"
        ></ColorfulPrice>
      </div>
      <div class="white-section__strip">
        <ColorfulStrip
          spanFrom="LIGHT"
          spanTo="PLUS"
          borderColor="#ff8f28"
          bgColor1="#ffca00"
          bgColor2="#ff8f28"
        >
          <template v-slot
            ><svg
              class="arrow arrow_second"
              width="286"
              height="25"
              viewBox="0 0 286 25"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M2.76172 10.4673C1.65715 10.4673 0.761719 11.3627 0.761719 12.4673C0.761719 13.5719 1.65715 14.4673 2.76172 14.4673V10.4673ZM285.904 12.4673L265.904 0.92028V24.0143L285.904 12.4673ZM2.76172 14.4673H267.904V10.4673H2.76172V14.4673Z"
                fill="white"
              />
            </svg> </template
        ></ColorfulStrip>
        <ColorfulPrice
          class="white-section__price"
          price="$105k"
          color="#ff8f28"
        ></ColorfulPrice>
      </div>
      <div class="white-section__strip">
        <ColorfulStrip
          spanFrom="PLUS"
          spanTo="PRO"
          borderColor="#ff4e68"
          bgColor1="#ff8f28"
          bgColor2="#ff4e68"
        >
          <template v-slot>
            <svg
              class="arrow arrow_third"
              width="405"
              height="24"
              viewBox="0 0 405 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M2.76172 10.3384C1.65715 10.3384 0.761719 11.2338 0.761719 12.3384C0.761719 13.4429 1.65715 14.3384 2.76172 14.3384V10.3384ZM404.793 12.3384L384.793 0.791373V23.8854L404.793 12.3384ZM2.76172 14.3384H386.793V10.3384H2.76172V14.3384Z"
                fill="white"
              /></svg></template
        ></ColorfulStrip>
        <ColorfulPrice
          class="white-section__price"
          price="$105k"
          color="#ff4e68"
        ></ColorfulPrice>
      </div>
      <div class="white-section__strip">
        <ColorfulStrip
          spanFrom="PRO"
          spanTo="ULTRA"
          borderColor="#8c35e3"
          bgColor1="#ff4e68"
          bgColor2="#8c35e3"
        >
          <template v-slot>
            <svg
              class="arrow arrow_fourth"
              width="500"
              height="24"
              viewBox="0 0 500 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M2.76172 9.64111C1.65715 9.64111 0.761719 10.5365 0.761719 11.6411C0.761719 12.7457 1.65715 13.6411 2.76172 13.6411V9.64111ZM499.803 11.6411L479.803 0.0941076V23.1881L499.803 11.6411ZM2.76172 13.6411H481.803V9.64111H2.76172V13.6411Z"
                fill="white"
              />
            </svg> </template
        ></ColorfulStrip>
        <ColorfulPrice
          class="white-section__price"
          price="$105k"
          color="#8c35e3"
        ></ColorfulPrice>
      </div>
    </div>

    <BlackText
      class="white-section__text"
      heading="CHOOSE YOUR PACKAGE!"
      text="Available on demand: the integration of AI and GPS functionality. Prices are available after consultation via example@example.com"
    ></BlackText>
    <div class="white-section__cards">
      <StartXCard></StartXCard>
      <LightCard></LightCard>
      <PlusCard></PlusCard>
      <ProCard></ProCard>
      <UltraSmallCard />
    </div>
  </div>
</template>
<style lang="scss">
.white-section {
  position: relative;
  &__picture {
    position: absolute;
    bottom: 2%;
    left: 100px;
    max-width: 300px;
  }
  &__price {
    margin: 0 auto;
  }
  &__strips {
    @include flex-column;
    gap: 14px;
  }
  &__strip {
    @include flex-column;
    gap: 10px;
  }
  &__cards {
    /* @include space-between-flex; */
    max-width: max-content;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 1fr;
    gap: 10px;
    padding: 0px 100px 350px 100px;
  }
  &__text {
    padding: 90px 100px 74px 100px;
  }
}
@media (max-width: 720px) {
  .arrow {
    width: 20px;
    &_second {
      width: 40px;
    }
    &_third {
      width: 80px;
    }
    &_fourth {
      width: 100px;
    }
  }
}

@media (min-width: 720px) and (max-width: 1160px) {
  .arrow {
    width: 100px;
    &_second {
      width: 150px;
    }
    &_third {
      width: 200px;
    }
    &_fourth {
      width: 250px;
    }
  }
  .white-section {
    &__cards {
      grid-template-columns: 1fr 1fr;
      gap: 20px;
      &__picture {
        bottom: 2%;
        left: 100px;
        max-width: 300px;
      }
    }
  }
}

@media (min-width: 1160px) {
  .white-section {
    &__strip {
      flex-direction: row;
      align-items: center;
      gap: 32px;
    }
    &__price {
      margin: 0 !important;
    }
    &__cards {
      grid-template-columns: 1fr 1fr 1fr;
    }
    &__picture {
      bottom: 4%;
      left: 100px;
      max-width: 400px;
    }
  }
}
@media (min-width: 1440px) {
  .white-section {
    &__picture {
      bottom: 6%;
      left: 100px;
      max-width: 600px;
    }
    &__strip {
      gap: 44px;
    }
    &__cards {
      grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
    }
  }
}
</style>
