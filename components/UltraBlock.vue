<template>
  <div class="ultra-block">
    <div class="ultra-block__part">
      <svg
        class="ultra-block__arrow"
        width="65"
        height="31"
        viewBox="0 0 65 31"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M2.28222 28.7251L32.2822 2.72507L62.2822 28.7251"
          stroke="white"
          stroke-width="4"
          stroke-linecap="round"
        />
      </svg>
    </div>
    <div class="ultra-block__content">
      <div>
        <span class="ultra-block__header">ULTRA</span>
        <p class="ultra-block__text">
          The most complete package of functions with maximum opportunities for
          the complete management of your business from anywhere in the world at
          any time!
        </p>
      </div>

      <div class="ultra-block__links">
        <span class="ultra-block__span">$300K</span>
        <div class="ultra-block__icons">
          <a href="/">
            <svg
              class="ultra-block__icon"
              width="39"
              height="39"
              viewBox="0 0 39 39"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M2.38428 10.4951H37.2769L35.3385 36.6646H4.32276L2.38428 10.4951Z"
                stroke="#8C35E3"
                stroke-width="3.22299"
                stroke-linejoin="round"
              />
              <path
                d="M12.0771 14.3721V1.77197H27.585V14.3721"
                stroke="#8C35E3"
                stroke-width="3.22299"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M12.0771 28.9106H27.585"
                stroke="#8C35E3"
                stroke-width="3.22299"
                stroke-linecap="round"
              />
            </svg>
          </a>
          <a href="/">
            <svg
              class="ultra-block__icon"
              width="32"
              height="31"
              viewBox="0 0 32 31"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M15.9629 1.64648V28.7901"
                stroke="#8C35E3"
                stroke-width="3.22299"
                stroke-linecap="round"
              />
              <path
                d="M29.5356 15.2184L2.39202 15.2184"
                stroke="#8C35E3"
                stroke-width="3.22299"
                stroke-linecap="round"
              />
            </svg>
          </a>
        </div>
      </div>
    </div>
    <div class="ultra-block__cards">
      <ColorfulCards />
      <monochrome-cards></monochrome-cards>
    </div>
  </div>
</template>

<style lang="scss">
.ultra-block {
  position: relative;
  padding: 80px 40px;
  margin-bottom: 90px;
  background-color: $primary;
  @include flex-column;
  gap: 100px;
  &__part {
    background-color: $primary;
    position: absolute;
    left: 25%;
    bottom: -4%;
    width: 165px;
    height: 87px;
    border-radius: 0 0 32px 32px;
  }
  &__arrow {
    position: absolute;
    margin-left: auto;
    margin-right: auto;
    left: 0;
    right: 0;
    top: 20%;
    max-width: 30px;
  }
  &__content {
    @include flex-column;
    gap: 30px;
    color: $white;
  }
  &__header {
    font-size: 32px;
    font-weight: 700;
  }
  &__text {
    font-size: 24px;
    line-height: 36px;
    letter-spacing: -3%;
  }
  &__cards {
    @include flex-column;
    align-items: center;
    gap: 100px;
  }
  &__links {
    background-color: $white;
    @include space-between-flex;
    align-items: center;
    border-radius: 12px;
    max-width: 450px;
  }
  &__span {
    color: $black;
    font-size: 24px;
    font-weight: 700;
    display: block;
    max-width: max-content;
    padding: 8px 40px 8px 30px;
    border-right: 2px solid $primary;
  }
  &__icons {
    @include center-flex;
    align-items: center;
    gap: 20px;
    padding: 10px;
  }
  &__icon {
    max-width: 20px;
  }
}
@media (min-width: 790px) {
  .ultra-block {
    padding: 120px 100px;
    @include center-flex;
    &__cards {
      flex-direction: row;
      @include center-flex;
      gap: 30px;
    }
    &__span {
      font-size: 32px;
    }
    &__header {
      font-size: 64px;
    }
    &__part {
      bottom: -6%;
    }
    &__icon {
      width: 40px;
    }
    &__arrow {
      max-width: 50px;
    }
  }
}
@media (min-width: 1440px) {
  .ultra-block {
    @include space-between-flex;
    flex-direction: row;
    &__span {
      font-size: 64px;
      padding: 10px 80px 10px 40px;
    }
    &__content {
      gap: 100px;
    }
    &__cards {
      margin-top: 100px;
      gap: 60px;
    }
    &__content {
      max-width: 450px;
    }
    &__header {
      font-size: 128px;
    }
    &__part {
      bottom: -8%;
    }
    &__arrow {
      max-width: 60px;
    }
  }
}
</style>
