<template>
    <div class= "input text-center">
        <label for="name">Nome completo: </label><br>
        <input type="text" id="name" name="name"><br><br>
        <a type="submit" class="btn btn-light" href="#usuarios">Enviar</a>
    </div>
</template>

<script>
export default {
    data: () => ({
        name: "InputNome",
    })
    
}

</script>

<style>
    .input {
        padding-top: 100px;
        font-family: 'Montserrat', sans-serif;
        color:#c3fada;
        
    }

</style>