<template>
  <head>
      <link href="https://fonts.googleapis.com/css2?family=Montserrat&display=swap" rel="stylesheet">
      <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
      <meta charset="utf-8">
      <meta name="viewport" content="width=device-width, initial-scale=1">

  </head>
    <HelloWorld/>
    <Table/>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Table from './components/Table.vue'

export default {
  
  components: {
    HelloWorld,
    Table
  }
}
</script>

<style>

</style>
