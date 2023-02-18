<template>
  <base-container title="Vuex">
    <h3>{{ $store.getters.finalCounter }}</h3>
    <favourite-value/>
    <button @click="addOne">add 1</button>
    <change-counter/>
  </base-container>
</template>

<script>
import BaseContainer from './components/BaseContainer.vue';
import ChangeCounter from './components/ChangeCounter.vue';
import FavouriteValue from './components/FavouriteValue.vue';

export default {
  components: {
    BaseContainer,
    ChangeCounter,
    FavouriteValue,
  },
  methods: {
    addOne() {
      this.$store.commit('increment');
    }
  },
};
</script>

<style>
* {
  box-sizing: border-box;
}

html {
  font-family: sans-serif;
}

body {
  margin: 0;
}
</style>