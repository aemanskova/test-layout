<template>
  <header class="header">
    <nav class="nav">
      <ul class="nav__links">
        <div class="nav__links_left">
          <li>ABOUT US</li>
          <li>TEAM</li>
          <li>PROJECTS</li>
        </div>
        <li>CONTACT US</li>
      </ul>
      <div class="nav__icons">
        <svg
          class="nav__icon"
          width="104"
          height="98"
          viewBox="0 0 104 98"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M1.875 0H88.875V63C88.875 76.8071 77.6821 88 63.875 88H26.875C13.0679 88 1.875 76.8071 1.875 63V0Z"
            fill="white"
          />
          <path
            d="M88.875 5.38604e-06L88.875 47.75C88.875 61.9873 88.875 69.1059 86.0603 74.5244C83.6884 79.0904 79.9654 82.8134 75.3994 85.1853C69.9809 88 62.8623 88 48.625 88L42.125 88C27.8877 88 20.7691 88 15.3506 85.1853C10.7846 82.8134 7.06156 79.0904 4.68967 74.5244C1.87501 69.1059 1.87501 61.9873 1.87501 47.75L1.87502 -2.20996e-06"
            stroke="white"
            stroke-width="2.17432"
          />
          <path
            d="M26.8145 36H62.8145L60.8145 63H28.8145L26.8145 36Z"
            stroke="black"
            stroke-width="4"
            stroke-linejoin="round"
          />
          <path
            d="M36.8145 40V27H52.8145V40"
            stroke="black"
            stroke-width="4"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M36.8145 55H52.8145"
            stroke="black"
            stroke-width="4"
            stroke-linecap="round"
          />
          <circle cx="86.0786" cy="80.4673" r="17.4673" fill="#FFCA00" />
          <path
            d="M88.6407 72.9789V88H85.6756V76.397L82.1134 77.5295V75.1925L88.3216 72.9789H88.6407Z"
            fill="black"
          />
        </svg>
        <svg
          class="nav__icon"
          width="91"
          height="100"
          viewBox="0 0 91 100"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M2 0H89V73C89 86.8071 77.8071 98 64 98H27C13.1929 98 2 86.8071 2 73V0Z"
            fill="#8C35E3"
          />
          <path
            d="M31.9029 40.064V47.52H40.0309V49.92H31.9029V57.6H40.9909V60H28.9909V37.664H40.9909V40.064H31.9029ZM61.9731 60H59.0611L47.3491 42.24V60H44.4371V37.664H47.3491L59.0611 55.392V37.664H61.9731V60Z"
            fill="white"
          />
          <path
            d="M89 1.11816e-05L89 57.75C89 71.9873 89 79.1059 86.1853 84.5244C83.8134 89.0904 80.0904 92.8134 75.5244 95.1853C70.1059 98 62.9873 98 48.75 98L42.25 98C28.0127 98 20.8941 98 15.4756 95.1853C10.9096 92.8134 7.18656 89.0904 4.81467 84.5244C2.00001 79.1059 2.00001 71.9873 2.00001 57.75L2.00002 2.72238e-06"
            stroke="white"
            stroke-width="2.17432"
          />
        </svg>
      </div>
    </nav>
  </header>
</template>
<style lang="scss" scoped>
.header {
  background-color: $primary;
  min-height: 200px;
}
.nav {
  @include center-flex;
  gap: 20px;
  &__links {
    letter-spacing: -3%;
    gap: 10px;
    padding-left: 0;
    align-items: flex-end;
    min-width: 240px;
    font-size: 12px;
    list-style-type: none;
    color: $white;
    @include space-between-flex;
    &_left {
      display: flex;
      gap: 10px;
    }
  }
  &__icons {
    display: flex;
    gap: 5px;
    margin-top: -35px;
  }
  &__icon {
    max-width: 30px;
  }
}

@media (min-width: 768px) {
  .header {
    min-height: 300px;
  }
  .nav {
    &__links {
      gap: 40px;
      min-width: 560px;
      font-size: 16px;
      margin-top: 40px;
      &_left {
        gap: 40px;
      }
    }
    &__icons {
      margin-top: -32px;
    }
    &__icon {
      max-width: 40px;
    }
  }
}
@media (min-width: 1440px) {
  .header {
    min-height: 400px;
  }
  .nav {
    gap: 60px;
    &__links {
      font-size: 24px;
      margin-top: 80px;
      min-width: 860px;
      &_left {
        gap: 60px;
      }
    }
    &__icon {
      max-width: 80px;
    }
    &__icons {
      margin-top: -12px;
      gap: 10px;
    }
  }
}
</style>
