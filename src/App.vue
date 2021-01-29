<template>
  <head>
      <link href="https://fonts.googleapis.com/css2?family=Montserrat&display=swap" rel="stylesheet">
      <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width, initial-scale=1">
  </head>
      <ul class="nav">
      
          <li class="nav-item">
            <a class="nav-link" href="#usuarios">Users</a>
          </li><li class="nav-item">
            <a class="nav-link" href="#todos">All</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#fotos">Photos</a>
          </li>
          <li class="nav-item">
            <a class="nav-link disabled" href="#">Disabled</a>
          </li>
      </ul>
    <HelloWorld/>
    <Table/>
    <TableAll/>
    <TablePhotos/>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Table from './components/Table.vue'
import TableAll from './components/TableAll'
import TablePhotos from './components/TablePhotos'

export default {
  
  components: {
    HelloWorld,
    Table,
    TableAll,
    TablePhotos
  }
}
</script>

<style>

</style>
