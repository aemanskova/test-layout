<template>
  <div class="strip">
    <div :style="bgStyle" class="strip__colorful-block">
      <span class="strip__text">{{ spanFrom }}</span>
      <slot></slot>
      <span class="strip__text">{{ spanTo }}</span>
    </div>
    <div :style="{ border: borderStyle }" class="strip__icons">
      <svg
        width="39"
        height="39"
        viewBox="0 0 39 39"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M1.86475 10.4785H36.7574L34.8189 36.648H3.80323L1.86475 10.4785Z"
          :stroke="borderColor"
          stroke-width="3.22299"
          stroke-linejoin="round"
        />
        <path
          d="M11.5576 14.3555V1.75537H27.0655V14.3555"
          :stroke="borderColor"
          stroke-width="3.22299"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M11.5576 28.894H27.0655"
          :stroke="borderColor"
          stroke-width="3.22299"
          stroke-linecap="round"
        />
      </svg>
      <svg
        width="31"
        height="31"
        viewBox="0 0 31 31"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M15.4434 1.62988V28.7735"
          :stroke="borderColor"
          stroke-width="3.22299"
          stroke-linecap="round"
        />
        <path
          d="M29.0161 15.2019L1.87248 15.2019"
          :stroke="borderColor"
          stroke-width="3.22299"
          stroke-linecap="round"
        />
      </svg>
    </div>
  </div>
</template>
<style lang="scss">
.strip {
  display: flex;
  &__colorful-block {
    padding: 0px 20px 0px 10px;
    display: flex;
    align-items: center;
    gap: 10px;
  }
  &__icons {
    background-color: #fff; /* Не было переменной $white, поэтому использовал #fff */
    display: flex;
    align-items: center;
    gap: 10px;
    padding: 5px 10px;
    border-radius: 0px 12px 12px 0px;
  }
  &__text {
    color: $white;
    font-size: 18px;
    font-weight: 700;
  }
}

@media (min-width: 790px) {
  .strip {
    &__colorful-block {
      padding: 10px 20px 10px 40px;
      gap: 20px;
    }
    &__text {
      font-size: 32px;
    }
    &__icons {
      padding: 26px 18px;
    }
  }
}
@media (min-width: 1160px) {
}
@media (min-width: 1440px) {
  .strip {
    &__colorful-block {
      padding: 24px 60px 24px 180px;
      gap: 40px;
    }
    &__text {
      font-size: 40px;
    }
    &__icons {
      padding: 36px 24px;
    }
  }
}
</style>

<script setup>
import { computed, ref } from "vue";
const props = defineProps({
  spanFrom: String,
  spanTo: String,
  borderColor: String,
  bgColor1: String,
  bgColor2: String,
});

const bgStyle = computed(() => {
  return {
    background: `linear-gradient(to right, ${props.bgColor1}, ${props.bgColor2})`,
  };
});

const borderStyle = ref(`2px solid ${props.borderColor}`);
</script>
