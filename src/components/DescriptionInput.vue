<template>
  <div class="message">
    <label for="name">Déscription : </label>
    <textarea name="message" id="message" cols="30" rows="10" required></textarea>
  </div>
</template>

<script>
export default {
  name: "DescriptionInput",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.message {
    display: flex;
    justify-content: center;
    margin-bottom: 30px;
}
</style>
