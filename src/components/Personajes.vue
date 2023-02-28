<script>
import axios from 'axios'

let API_URL = 'https://rickandmortyapi.com/api/character'

export default {

  data() {
    return {
      info: [],
      personajes: [],
      cont:1,
    }
  },

  mounted() {
    axios.get(API_URL)
      .then((response) => {
        this.info = response.data.info;
        this.personajes = response.data.results;
      })
  },

  methods: {
    pag(num) {
      API_URL='https://rickandmortyapi.com/api/character/?page='+this.cont
      console.log(API_URL)
      axios.get(API_URL)
      .then((response) => {
        console.log(response.config)
        this.info = response.data.info;
        this.personajes = response.data.results;
      })
    }
  },

}

</script>

<template>
  <h2>Hay {{ info.count }} personajes en el programa de Rick & Morty</h2>
  <br>
  <ul class="pl-5">
    <li v-for="p in personajes">
      <button @click="" class="my-2">{{ p.name }}</button>
    </li>
  </ul>
  <button  v-if="cont > 1" @click="pag(cont--)" class="my-5 bg-green-200 rounded-lg text-lg mx-5">Regresar</button>
  <button>{{ count }}</button>
  <button v-if="cont <= 42" @click="pag(cont++)" class="my-5 bg-green-200 rounded-lg text-lg mx-5">Siguiente</button>
</template>