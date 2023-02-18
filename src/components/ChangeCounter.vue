<template>
  <button @click="addOne"> Cc button </button>
</template>

<script>
export default {
    methods: {
        addOne() {
            this.$store.commit('increment');
        }
    }
}
</script>

<style>

</style>