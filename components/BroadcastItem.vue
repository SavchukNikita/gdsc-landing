<template lang="pug">
  article( class="broadcast-item" )
    v-card( class="broadcast-item__card" )
      .broadcast-item__img
        img(src="../assets/images/yt.png" alt="yuotube preview" class="broadcast-item__img-inner" )
      v-card-title( class="text" ) DevOps воркшоп - 13.05
      v-card-text Разобрали что-то там, а что-то не разбирали. Как-то так в общем и целом.
</template>

<style lang="scss" scoped>
  .broadcast-item {
    flex: 1 300px;
    margin: 24px;
    &__card {
      background-color: var(--v-primary-base);
    }

    &__img {
      width: 100%;
    }

    &__img-inner {
      width: 100%;
      height: auto;
    }
  }

  @media (min-width: 1025px) {
    .broadcast-item {
      max-width: 300px;
    }
  }
</style>
