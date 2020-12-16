<template>
    <!-- news -->
    <div class="row mt-md-5 mt-sm-5 mt-xs-5" >
        <div class="col-lg-6 col-xs-12" v-for="(noticia, index) of noticias" :key="index">
            <div class="d-flex justify-content-center align-items-center" >

                <div class="p-3">
                    <img :src="noticia.image" alt="Foto noticia" height="200" width="350">
                </div>

                <div class="p-2">
                    <h4>{{noticia.title}}</h4>
                    <p>
                        {{noticia.description}}
                    </p>
                </div>

            </div>
            <div class="d-flex container-fluid justify-content-end pb-2 mt-n2" >
                <a :href="noticia.url" class="btn btn-info" target="_blank">Más información...</a>
            </div>
        </div>
    </div>
        
</template>

<script>
import axios from 'axios'

export default {
    name:"NewsSections",
    data(){
        return{
            noticias: null
        }
        
    },
    created(){
        axios
            .get(`https://gnews.io/api/v4/top-headlines?token=b3e26d1fb381b28584899c569b80e702&topic=science`)
            .then( response =>{this.noticias = response.data.articles.slice(0,4)})        

    }

};
</script>

<style scoped>
</style>