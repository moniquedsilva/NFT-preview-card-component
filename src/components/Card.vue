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
    <div class="card__info">
      <img src="assets/images/image-avatar.png" alt="Avatar" />
      <p><span>Creation of</span> Jules Wyvern</p>
    </div>
  </article>
</template>

<style lang="scss">
.card {
  background-color: $dark-blue-2;
  border-radius: 15px;
  display: flex;
  flex-direction: column;
  gap: 1.75rem;
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
