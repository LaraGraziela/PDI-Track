<template>
  <head>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    
  
  </head>
    <div class="row">
      
        <div class="col-sm-6">
          <h2 class="titulo">Cadastro de Costumer </h2>

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

          <img src="../assets/mesa.png" class="mx-auto d-block" alt="" width="400" height="400" id="png3">

        </div>

        <div class="col-sm-6">
          <div class="formulario container-fluid">
            <form class="was-validated form">
               
                <input class="form-control input" type="text" id="name" name="name" required placeholder="Nome completo"><br><br>

                  
                <input class="form-control input" type="email" id="email" name="email" required placeholder="Email"><br><br>

                  
                <input class="form-control input" type="text" id="cpf" name="cpf" required placeholder="CPF"><br><br>

                <label for="dataNasc">Data de nascimento:</label><br>
                <input class="form-control input" type="date" id="dataNasc" name="dataNasc" required><br><br>

                  
                <input class="form-control input" type="tel" id="phone" name="phone" pattern="[0-9]({2})[0-9]{5}-[0-9]{4}" required placeholder="Telefone"><br><br>

                <label for="country">Cargo:</label><br>
                <select class="form-control" id="cargo" name="cargo">
                  <option value="none">Selecione o cargo</option>
                  <option value="analistaReq">Analista de Requisitos</option>
                  <option value="gerenteVend">Gerente de Vendas</option>
                  <option value="liderFinan">Líder Financeiro</option>
                  <option value="vendedor">Vendedor</option>
                </select><br>

                  
                <input class="form-control input" type="password" id="password" name="password" required placeholder="Senha"><br>
                <button type="submit" class="btn btn-light">Cadastrar</button><br><br>
            </form>       
          </div>
        
      </div>
    </div>  
      <hr>

</template>

<script>
export default {
  data:()=> ({
  id: "",
  name: "name",
  email: "email",
  cpf: "cpf",
  dataNasc: "dataNasc",
  phone: "phone",
  cargo: "cargo",
  
})
}

</script>


<style>
  body {
    background-image: linear-gradient( #1cd381,#19b16c);
  }
  .formulario {
    font-family: 'Montserrat', sans-serif;
    text-align: left;
    font-size: 15px;
    padding: 50px;
  
  }
  
  .titulo{
    text-align: center;
    padding-top: 100px;
    font-size: 45px;
    font-family: 'Montserrat', sans-serif;
    color:#c3fada;
    
  }

  .form{
    padding-left: 200px;
    padding-right: 200px;
    size: 10px;
    font-size: 20px;
  }
  
  div.box {
    width: 160px;
    display: inline-block;
    padding-top: 100px;
    padding-left: 100px;
  }

  #png{

  }
</style>
