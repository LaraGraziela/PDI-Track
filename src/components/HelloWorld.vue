<template>
  <div class="formulario">
    <h1>Cadastro de Costumers</h1> 
    <form>
        <label for="name">Nome completo:</label><br>
        <input type="text" id="name" name="name"><br><br>

        <label for="email">Email:</label><br>
        <input type="email" id="email" name="email"><br><br>

        <label for="cpf">CPF:</label><br>
        <input type="text" id="cpf" name="cpf"><br><br>

        <label for="dataNasc">Data de nascimento:</label><br>
        <input type="date" id="dataNasc" name="dataNasc"><br><br>

        <label for="phone">Telefone:</label><br>
        <input type="tel" id="phone" name="phone" pattern="[0-9]({2})[0-9]{5}-[0-9]{4}"><br><br>

        <label for="cargo">Cargo:</label><br>
        <input type="radio" id="cargo" name="cargo">
        <label for="cargo"> Analista de Requisitos</label><br>
        <input type="radio" id="cargo" name="cargo">
        <label for="cargo"> Assistente de Vendas</label><br>
        <input type="radio" id="cargo" name="cargo">
        <label for="cargo"> Estágio Front-end</label><br>
        <input type="radio" id="cargo" name="cargo">
        <label for="cargo"> Analista Contábil</label><br><br>

        <label for="password">Senha padrão (inicial):</label><br>
        <input type="password" id="password" name="password"><br>
        
    </form><br>

    <button type="submit" onclick="alert ('Cadastro Realizado')">Cadastrar</button><br><hr><br>
    </div>

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

</style>
