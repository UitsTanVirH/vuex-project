<template>
  <p>Do more... </p>
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