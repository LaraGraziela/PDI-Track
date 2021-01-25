<template>
    <div class="tabela">
        <h1>Customers Cadastrados</h1>

        <table style="width:100%">
            <tr>
                <th>ID</th>
                <th>Nome</th>
                <th>Email</th>
                <th>CPF</th>
                <th>Data de nascimento</th>
                <th>Cargo</th>
            </tr>
            <tr>
                <td></td>
                <td>Lara</td>
                <td>Smith</td>
                <td>50</td>
            </tr>
            <tr>
                <td></td>
                <td>Eve</td>
                <td>Jackson</td>
                <td>94</td>
            </tr>
        </table>
  
    </div>
</template>

<script>
export default {
    
}
</script>

<style>
 table, th, td {
  border: 1px solid rgb(153, 153, 153);
  border-collapse: collapse;
}
th, td {
  padding: 15px;
}

</style>