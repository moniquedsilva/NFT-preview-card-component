<template>
  <article class="card">
    <h1 class="card__title">Equilibrium #3429</h1>
    <p class="card__paragraph">
      Our Equilibrium collection promotes balance and calm.
    </p>
    <img
      src="assets/images/image-equilibrium.jpg"
      alt="Equilibrium"
      class="card__image"
    />
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
  border-radius: 15px;
  box-shadow: 0px 28px 5px 15px hsla(217, 55%, 10%, 1);
  display: flex;
  flex-direction: column;
  gap: 1.625rem;
  padding: 1.5rem;
  width: 87%;
  height: 37.25rem;
  &__title {
    color: $white;
    font: 600 1.3125rem $outfit;
  }
  &__paragraph {
    color: $blue;
    font: $outfit-size $outfit;
  }
  &__image {
    order: -1;
    border-radius: 15px;
  }
  &__timestamp {
    display: flex;
    justify-content: space-between;
    align-items: center;
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
  }
}
</style>
