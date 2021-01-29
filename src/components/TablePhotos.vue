<template>
    <head>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
     
  </head>

  <div class="row" id="fotos">
            <div class="col-sm-12">
                <div class="container">
                    <h1 class="tituloTable">PHOTOS</h1>

                    <table class="tabela table-bordered formulario" style="width:100%">
                        <thead>
                            <th>Album ID</th>
                            <th>ID</th>
                            <th>Title</th>
                            <th>URL</th>
                            <th>Thumbnail</th>
                        </thead>
                        <thead v-for="(photos,index) in fotos" :key="index">
                         
                            <td>{{photos.albumId}}</td>
                            <td>{{photos.id}}</td>
                            <td>{{photos.title}}</td>
                            <td>{{photos.url}}</td>
                            <td>{{photos.thumbnailUrl}}</td>
                        </thead>
                    </table>
            
                </div>
            </div>
        </div>   
     
</template>

<script>
import axios from "axios";
export default {
    data: () => ({
        fotos: null,
        ability: null
    }),
    created: function () {
        axios.get("https://jsonplaceholder.typicode.com/photos")
        .then(res=>{
            this.fotos = res.data
            console.log(this.fotos)
        })
    }
    
}
</script>

<style>

</style>