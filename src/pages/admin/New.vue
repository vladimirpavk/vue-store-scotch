<template>
  <div>
    <div class="title">
      <h1>This is Admin/New</h1>
    </div>
    <label for="name">Unesite ime(obavezno polje) : </label>
    <input type="text" placeholder="Imex" v-model="model.ime" v-validate="'required'" name="name"/>
    <div>
      <button v-on:click="validate()">Validate</button>
    </div>
  </div>     
</template>
<script>
  export default{
    name: 'New',
    data () {
      return {
        model: {
          ime: 'Vlada'
        }
      }
    },
    methods: {
      validate () {
        console.log(this.model.ime)
        console.log(this.errors)
      }
    }
  }
</script>