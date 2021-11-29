<template>
<h1>Formulaire d'inscription</h1>
<div v-if="step === 'step-1'">
  <h2>Etape 1 :</h2>
  <TextInput msg= "nom" />
  <RadioInput msg= "radio" />
  <ButtonNext msg= "" v-on:click="step='step-2'"/>
</div>
<div v-if="step === 'step-2'">
  <h2>Etape 2 :</h2>
  <DateInput msg= "date" />
  <SelectInput msg= "select" />
  <ButtonNext msg= "" v-on:click="step='step-3'"/>
</div>
<div v-if="step === 'step-3'">
  <h2>Etape 3 :</h2>
  <DescriptionInput msg= "description" />
  <ButtonInput msg= "button" />
</div>

  
</template>

<script>
import TextInput from './components/TextInput'
import DateInput from './components/DateInput'
import DescriptionInput from './components/DescriptionInput'
import RadioInput from './components/RadioInput'
import SelectInput from './components/SelectInput'
import ButtonInput from './components/ButtonInput'
import ButtonNext from './components/ButtonInput'

export default {
  name: 'App',
  components: {
    TextInput,
    DescriptionInput,
    SelectInput,
    DateInput,
    RadioInput,
    ButtonInput,
    ButtonNext
  },
  data () {
    return {
      step: 'step-1'
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
