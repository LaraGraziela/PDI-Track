<template>
    
    <head>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">    
  
  </head>

    <div class="row">
            <div class="col-sm-12" id="todos">
                <div class="container">
                    <h1 class="tituloTable">ALL</h1>

                    <table class="tabela table-bordered formulario" style="width:100%">
                        <thead>
                            <th>User ID</th>
                            <th>ID</th>
                            <th>Title</th>
                            <th>Completed</th>
                        </thead>
                        <thead v-for="(all,index) in todos" :key="index">
                            
                            <td>{{all.userId}}</td>
                            <td>{{all.id}}</td>
                            <td>{{all.title}}</td>
                            <td>{{all.completed}}</td>
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
        todos: null
    }),
    created: function (){
        axios.get('https://jsonplaceholder.typicode.com/todos')
        .then(res=> {
            this.todos = res.data
            console.log(this.todos)

        })
    }
    
}
</script>

<style>

</style>