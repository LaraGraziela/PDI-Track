<template>
  <head>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
   
  </head>
    <div class="row">
      
        <div class="col-sm-6">
          <h2 class="titulo">INPUT E USERS </h2>

          <div class="box">
            <img src="../assets/usuario1.png" class="mx-auto d-block" alt="" width="200" height="200" id="png">
          </div>
          <div class="box">
            <img src="../assets/usuario3.png" class="mx-auto d-block" alt="" width="200" height="200" id="png1">
          </div>
          <div class="box">
            <img src="../assets/usuario4.png" class="mx-auto d-block" alt="" width="200" height="200" id="png2">
          </div>
          <div class="box">
            <img src="../assets/usuario5.png" class="mx-auto d-block" alt="" width="200" height="200" id="png3">
          </div>    
        

        </div>

          <div class="col-sm-6"> 
             
            <InputNome/>
       
          </div>
    </div>
    <br><br><br><br><br><br><br>  
    <hr>

</template>

<script>
import InputNome from './InputNome'

export default {
  components: {
    InputNome
  }
}

</script>


<style>
  body {
    background-image: linear-gradient( #1cd381,#19b16c);
  }
  
  .titulo{
    text-align: center;
    padding-top: 50px;
    font-size: 45px;
    font-family: 'Montserrat', sans-serif;
    color:#c3fada;
    margin-left: 131px;
    
  }
  
    .box {
    width: 160px;
    display: inline-block;
    padding-top: 100px;
    padding-left: 100px;
  }

</style>
