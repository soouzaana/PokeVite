<script setup>
const pokemon = defineProps(["name", "urlBaseSvg"]);
</script>

<template>
  <div class="col-4">
    <div class="card p-2 mb-3 cardListPokemon">
      <p class="text-center">{{ pokemon.name }}</p>
      <img :src="urlBaseSvg" class="card-img-top" alt="..." height="100rem" />
    </div>
  </div>
</template>

<style scoped>
.cardListPokemon {
  background: #f78a9e;
  background: radial-gradient(
    circle,
    rgba(240, 73, 142, 0.3) 0%,
    rgba(218, 112, 161, 0.2) 100%
  );
  cursor: pointer;
}

.cardListPokemon:hover{
  background: #f78a9e;
  background: radial-gradient(
    circle,
    rgba(240, 73, 142, 0.6) 0%,
    rgba(218, 112, 161, 0.3) 100%
  );
}

.cardListPokemon img:hover{
  padding: .1rem;
}
</style>
