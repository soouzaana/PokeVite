<script setup>
const pokemon = defineProps(["name", "xp", "height", "img", "loading", "abilities", "game_index"]);
</script>

<template>
  <div>
    <div
      class="card CardPokemonSelected p-5"
      :class="loading ? '' : 'animate__animated animate__flipInY'"
    >
      <img
        v-if="pokemon.name"
        :src="pokemon.img"
        class="card-img-top pt-2"
        :alt="pokemon.name"
        height="250rem"
      />
      <img
        v-else
        src="../assets/egg_pokemon.svg"
        class="card-img-top pt-2"
        alt="???"
        height="250rem"
      />
      <div class="card-body">
        <h5 class="card-title text-center">{{ pokemon.name || '???' }}</h5>
        <hr />
        <div class="row">
          <section class="col">
            <strong>Número: </strong>
            <span>{{pokemon.game_index}}</span>
          </section>
          <section class="col">
            <strong>XP: </strong>
            <span>{{pokemon.xp}}</span>
          </section>
          <section class="col">
            <strong>Altura: </strong>
            <span>{{pokemon.height}}</span>
          </section>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.CardPokemonSelected {
  background: #ffb28f;
  background: radial-gradient(circle, #ff578fab 0%, #ffb38fe8 100%);
  height: 75vh;
}
</style>
