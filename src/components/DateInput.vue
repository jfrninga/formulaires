<template>
  <div class="date">
    <label for="name">Date : </label>
    <input id="date" type="date" value="2021-11-24" required />
  </div>
</template>

<script>
export default {
  name: "DateInput",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.date {
    margin-bottom: 30px;
}
</style>
