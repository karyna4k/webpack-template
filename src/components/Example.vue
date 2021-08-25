<template>
  <section>
    <div class="container">
      <h1>{{ message }}</h1>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      message: null,
    };
  },
  created() {
    this.message = this.$store.getters.getMessage;
  },
};
</script>

<style lang="scss" scoped>
h1 {
  color: #41b883;
  text-align: center;
}
</style>