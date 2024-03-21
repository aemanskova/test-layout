<style lang="scss" scoped>
.form {
  max-width: 468px;
  width: 100%;
  &__fieldset {
    border: 0;
    margin: 0;
    min-width: 0;
    padding: 0.01em 0 0 0;
    @include flex-column;
  }
  &__header {
    color: $white;
    font-size: 18px;
    font-weight: 700;
    margin-bottom: 30px;
  }
  &__inputs {
    @include flex-column;
    gap: 24px;
  }
  &__input {
    all: unset;
    background-color: $white;
    padding: 22px 25px;
    border-radius: 20px;
    width: max-content;
    &::placeholder {
      color: $primary;
      font-size: 16px;
    }
  }
  &__block {
    margin-top: 20px;
    position: relative;
    max-width: max-content;
  }
  &__picture {
    position: absolute;
    max-width: 80px;
    bottom: 86%;
    left: 60%;
  }
  &__button {
    max-width: max-content;
    border: none;
    padding: 0;
    border: 2px solid $black;
    background-color: $white;
    color: $black;
    padding: 22px 80px;
    border-radius: 20px;
    font-size: 16px;
    font-weight: 700;
  }
  &__span {
    font-size: 16px;
    color: $white;
    margin: 17px 0px 37px 38px;
    &_underlined {
      text-decoration: underline;
      margin-left: 0px;
    }
  }
}
@media (min-width: 790px) {
  .form {
    &__header {
      font-size: 24px;
    }
    &__picture {
      bottom: 65%;
      left: 45%;
      max-width: 200px;
    }
    &__input {
      width: 100%;
    }
    &__block {
      max-width: 100%;
      margin-top: 100px;
    }
  }
}
@media (min-width: 1440px) {
  .form {
    &__header {
      font-size: 32px;
    }
    &__picture {
      max-width: 280px;
      bottom: 50%;
      left: 54%;
    }
    &__block {
      margin-top: 0px;
    }
  }
}
</style>
<template>
  <form class="form" action="">
    <fieldset class="form__fieldset">
      <legend class="form__header">ANY QUESTIONS?</legend>
      <div class="form__inputs">
        <div class="form__block">
          <label for="name" hidden>Name</label>
          <input id="name" class="form__input" type="text" placeholder="Name" />
          <img class="form__picture" src="/img/footer-girl.png" alt="" />
        </div>

        <label for="email" hidden>Email</label>
        <input
          id="email"
          class="form__input"
          type="email"
          placeholder="E-mail"
        />
        <label for="message" hidden>Your message</label>
        <input
          id="message"
          class="form__input"
          type="text"
          placeholder="Your message"
        />
      </div>

      <span class="form__span"
        >I agree with
        <span class="form__span form__span_underlined"
          >privacy policy</span
        ></span
      >
      <button class="form__button" type="submit">SEND</button>
    </fieldset>
  </form>
</template>
