<template>
  <footer class="footer">
    <p class="footer__paragraph">
      Challenge by
      <a
        href="https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U"
        target="_blank"
        class="footer__link"
        >Frontend Mentor</a
      >. Coded by
      <a
        href="https://github.com/moniquedsilva"
        target="_blank"
        class="footer__link"
        >Monique Silva</a
      >.
    </p>
  </footer>
</template>

<style lang="scss">
.footer {
  position: absolute;
  bottom: 1%;
  text-align: center;
  width: 87%;
  &__paragraph {
    color: $white;
    font-family: $outfit;
  }
  &__link {
    color: $blue;
  }
}
</style>
