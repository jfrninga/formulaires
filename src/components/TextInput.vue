<template>
  <div class="main-data">
    <div class="data-1">
      <label for="name">Nom : </label>
      <input type="text" id="name" name="user_name" required />
    </div>
    <div class="data-2">
      <label for="name">Prénom : </label>
      <input type="text" id="firstname" name="user_firstname" required />
    </div>
  </div>
</template>

<script>
export default {
  name: "Textinput",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.main-data {
  padding-top: 20px;
}

.data-1 {
        margin: 10px;
  }
.data-2 {
        margin: 20px;
        padding-right: 20px;
  }
</style>
