<template>
  <div id="app">

    <div class="container-fluid">
        <div class="row justify-content-center mb-5">
          <div class="col mt-5" v-for="(item, index) of team" :key="index">
            <team-card></team-card>
          </div>
        </div>
    </div>

    <page-footer></page-footer>
  </div>
</template>

<script>

import PageFooter from './components/PageFooter.vue'
import TeamCard from './components/TeamCard.vue'


export default {
  name: 'App',
  components:{
    PageFooter,
    TeamCard
  },
  data(){
    return{
      title : 'Vivo dentro de VUE',
      team:[
        {
          codigo: 1,
          nombre: "Primer Integrante",
          descripcion:
            "lorem ipsum",
          rol: "Desarrollador backend",
          imagen: "https://placeimg.com/192/192/people",
        },
        {
          codigo: 2,
          nombre: "Segundo Integrante",
          descripcion:
          "lorem ipsum",
          rol: "Desarrollador backend",
          imagen: "https://placeimg.com/192/192/people",
        },
        {
          codigo: 3,
          nombre: "Tercer Integrante",
          descripcion:
          "lorem ipsum",
          rol: "Desarrollador backend",
          imagen: "https://placeimg.com/192/192/people",
        },
        {
          codigo: 4,
          nombre: "Cuarto Integrante",
          descripcion:
          "lorem ipsum",
          rol: "Desarrollador backend",
          imagen: "https://placeimg.com/192/192/people",
        },
        {
          codigo: 5,
          nombre: "Quinto Integrante",
          descripcion:
          "lorem ipsum",
          rol: "Desarrollador backend",
          imagen: "https://placeimg.com/192/192/people",
        }
      ]
    }
  }
}
</script>

