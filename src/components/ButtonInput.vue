<template>
<div class="btn">
  <button v-on:click="$emit('validation')">Valider</button>
</div>
  
</template>

<script>
export default {
  name: "ButtonInput",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .btn {
    margin-top: 30px;
  }
</style>
