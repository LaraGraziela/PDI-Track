<template>
    <head>
        <link href="https://fonts.googleapis.com/css2?family=Montserrat&display=swap" rel="stylesheet"> 
        <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">
    </head>
        <div class="row" id="usuarios">
            <div class="col-sm-12">
                <div class="container-fluid">
                    <h1 class="tituloTable">USERS</h1>

                    <table class="tabela table-bordered formulario" style="width:100%">
                        <thead>
                            <th>ID</th>
                            <th>Name</th>
                            <th>Username</th>
                            <th>Email</th>
                            <th>Adress</th>
                            <th>Phone</th>
                            <th>Website</th>
                            <th>Company</th>
                        </thead>
                        <thead v-for="(user,index) in usuarios" :key="index">
                            <td>{{user.id}}</td>
                            <td>{{user.name}}</td>
                            <td>{{user.username}}</td>
                            <td>{{user.email}}</td>
                            <td>
                                Street: {{user.address.street}} <br>
                                Suite: {{user.address.suite}}<br>
                                City: {{user.address.city}}<br>
                                Zipcode: {{user.address.zipcode}}<br>                  
                            </td>
                            <td>{{user.phone}}</td>
                            <td>{{user.website}}</td>
                            <td>Name: {{user.company.name}} <br>
                                CatchPhrase: {{user.company.catchPhrase}} <br>
                                
                            </td>
                        </thead>
                    </table>
            
                </div>
            </div>
        </div>    
</template>

<script>
import axios from "axios"
export default {
    data: ()=> ({
        usuarios: null
    }),
    created: function (){
        axios.get('https://jsonplaceholder.typicode.com/users')
        .then(res=> {
            this.usuarios = res.data
            console.log(this.usuarios.adress)

        })
    }
    
}
</script>

<style>
.tituloTable{  
   text-align: center;
   padding: 50px;
   font-family: 'Montserrat', sans-serif;
   color: #c3fada;
    
}
th, td {
  padding: 20px;
  color: rgb(105, 105, 105);
}

.tabela{
    padding-bottom: 50px;
    background-color: white;
}

</style>