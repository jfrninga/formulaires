<template>
  <div class="container">
    <div class="sexe">
      <label for="huey">Homme</label>
      <input type="radio" id="sexe" name="sexe" value="homme" checked required />
    </div>
    <div class="sexe">
      <label for="huey">Femme</label>
      <input type="radio" id="sexe" name="sexe" value="femme" checked required />
    </div>
  </div>
</template>

<script>
export default {
  name: "RadioInput",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
    display: flex;
    justify-content: center;
}
.sexe {
    padding: 5px;
    margin-bottom: 15px;
}

</style>
