<template>
   
    <div class="card text-white bg-info">
        <div class="d-flex justify-content-center p-2">
            <img :src="member.image" alt="Foto equipo" height="200" width="200">
            
        </div>
        <div class="card-body">
            <h5 class="card-title">{{member.nombre}}</h5>
            <p class="card-text"> {{member.descripcion}}</p>
        </div>
        <div class="card-footer">
            <small class="text-white" > {{member.codigo}}. {{member.rol}}</small>
        </div>
    </div>

</template>

<script>
    export default {
        name: "TeamCard",
        props:['member']
    }
</script>

<style scoped>

</style>
