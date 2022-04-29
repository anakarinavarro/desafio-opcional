<template>
<div>
<h1>Desafío Opcional Vue Cli</h1>

<table class="table table-striped">
  <thead>
    <tr>
      
      <th scope="col">Nombre</th>
      <th scope="col">Apellido</th>
      <th scope="col">Run</th>
      <th scope="col">Fecha de nacimiento</th>
      <th scope="col">Edad</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="(usuario, $index) of usuarios" :key="$index">
      <td>{{usuario.nombre}}</td>
      <td>{{usuario.apellido}}</td>
      <td>{{usuario.run}}</td>
      <td>{{usuario.nacimiento}}</td>
      <td>{{usuario.edad}}</td>
    </tr>
  </tbody>
</table>
</div>

</template>

<script>
export default {
  name: 'App',
  data: ()=>({
    usuarios: [
      {nombre:"Jose", apellido:"Perez", run:"123456-2", nacimiento:"12-04-67", edad:"52"},
      {nombre:"Maria", apellido:"Rodriguez", run:"654321-1", nacimiento:"30-11-90", edad:"29"},
      {nombre:"Manuel", apellido:"Patiño", run:"14223456-6", nacimiento:"02-12-59", edad:"60"}
    ]
  })
}
</script>

<style>

</style>
