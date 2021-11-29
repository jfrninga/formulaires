<template>
  <label for="select">Catégories : </label>
  <select v-model="selected" v-on:click="$emit('changer')" required>
      <!-- <span>Selected: {{ selected }}</span> -->
    <option v-for="option in options" v-bind:value="option.value" v-bind:key="option.text">
      {{ option.text }}
    </option>
  </select>
  
</template>

<script>
export default {
  name: "SelectInput",
  props: {
    msg: String,
  },
  data() {
    return {
      selected: "A",
      options: [
        { text: "Etudiant", value: "A", colories: 'yellow' },
        { text: "Professionnel", value: "B", colories: 'grey' },
        { text: "Stagiaire", value: "C", colories: 'blue' },
        { text: "alternant", value: "D", colories: 'black' },
      ],
    };
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
}
</style>



    