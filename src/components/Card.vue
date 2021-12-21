<template>
  <article class="card">
    <h1 class="card__title">Equilibrium #3429</h1>
    <p class="card__paragraph">
      Our Equilibrium collection promotes balance and calm.
    </p>
    <picture class="card__image">
      <img
        src="assets/images/image-equilibrium.jpg"
        alt="Equilibrium"
        class="card__equilibrium"
      />
    </picture>
    <div class="card__timestamp timestamp">
      <div class="timestamp__info">
        <img src="assets/icons/icon-ethereum.svg" alt="Ethereum icon" />
        <span class="timestamp__money">0.041 ETH</span>
      </div>
      <div class="timestamp__info">
        <img src="assets/icons/icon-clock.svg" alt="Clock" />
        <span class="timestamp__time">3 days left</span>
      </div>
    </div>
    <div class="card__profile">
      <img
        src="assets/images/image-avatar.png"
        alt="Avatar"
        class="card__avatar"
      />
      <p class="card__autor">
        Creation of <span class="card__name">Jules Wyvern</span>
      </p>
    </div>
  </article>
</template>

<style lang="scss">
.card {
  background-color: $dark-blue-2;
  border-radius: 1rem;
  box-shadow: 0px 28px 5px 15px hsla(217, 55%, 10%, 1);
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  gap: 1.4rem;
  padding: 1.5rem;
  width: 87%;
  &__title {
    color: $white;
    cursor: pointer;
    font: 600 1.3125rem $outfit;
    width: max-content;
    margin: 0;
  }
  &__title:hover {
    color: $cyan;
  }
  &__paragraph {
    color: $blue;
    font: $outfit-size $outfit;
  }
  &__equilibrium {
    border-radius: 0.5rem;
    width: 100%;
  }
  &__image {
    cursor: pointer;
    display: block;
    order: -1;
    position: relative;
    width: 100%;
  }
  &__image::before {
    content: '';
    background: url('../../public/assets/icons/icon-view.svg') center no-repeat
      #fff;
    background-color: hsla(178, 100%, 50%, 0.5);
    border-radius: 0.5rem;
    display: block;
    position: absolute;
    top: 0;
    right: 0;
    bottom: 0;
    left: 0;
    z-index: 100;
    opacity: 0;
    visibility: hidden;
    transition: visibility 0.5s, opacity 0.5s;
  }
  &__image:hover::before,
  &__image:active::before {
    opacity: 1;
    visibility: visible;
  }
  &__timestamp {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }
  &__profile {
    border-top: 1px solid $dark-blue-3;
    display: flex;
    align-items: center;
    gap: 1rem;
    padding-top: 0.875rem;
  }
  &__avatar {
    border-radius: 100%;
    cursor: pointer;
    outline: 1px solid $white;
    width: 2rem;
  }
  &__autor {
    color: $blue;
    font: 1rem $outfit;
  }
  &__name {
    color: $white;
    cursor: pointer;
  }
  &__name:hover {
    color: $cyan;
  }
}

.timestamp {
  &__info {
    display: flex;
    gap: 0.375rem;
    align-items: center;
  }
  &__money {
    color: $cyan;
    font: 600 $outfit-size $outfit;
    letter-spacing: 1px;
  }
  &__time {
    color: $blue;
    font: $outfit-size $outfit;
  }
}

@media (min-width: $desktop) {
  .card {
    width: 21.875rem;
    gap: 1.625rem;
  }
}
</style>
