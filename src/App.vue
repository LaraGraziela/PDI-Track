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
      </ul>
      <div class="container-fluid">
          <Form/>
          <Table/>
      </div>
      <TableAll/>
      <TablePhotos/>

</template>

<script>
import Form from './components/Form'
import Table from './components/Table'
import TableAll from './components/TableAll'
import TablePhotos from './components/TablePhotos'

export default {
  
  components: {
    Form,
    Table,
    TableAll,
    TablePhotos
  }
}
</script>

<style>

</style>
