<template>
    <div>
        <h5 class="card-title">Peliculas que {{nombre}} desea ver (otra vez)</h5>
        <ul>
            <li v-for="(pelicula,i) in peliculas" v-bind:key="i">{{i+1}}. {{pelicula}}</li>
        </ul>
    </div>
</template>
<script>
export default {
    name: 'MiLista',
  props: {
    msg: String
  },
  data:function(){
    return{
      nombre:'JP',
      peliculas:['Pacific Rim','Jurassic Park','Back to the Future','Dawn of the dead','Police Academy']
    }
  }
}
</script>
<style scoped>
    li {
        background-color: red;
    }
</style>