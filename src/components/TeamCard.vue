<template>
    <div>
        <div class="card text-white bg-dark">
            <div class="d-flex justify-content-center p-2">
               <img v-bind:src="member.imagen" alt="Fotografía del equipo" >
            </div>
            <div class="card-body">
                <h5 class="card-title">{{ member.nombre }}</h5>
                <p class="card-text">{{ member.descripcion }}</p>
                <p class="card-text"><span>Rol: </span>{{ member.rol }}</p>
                <p class="card-text"><span>Código: </span>{{ member.codigo }}</p>
            </div>
            <div class="card-footer">
                <small class="text-muted">Last updated 3 mins ago</small>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>

</style>
