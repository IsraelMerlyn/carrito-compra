<template>
    <div class="col-md-6 col-lg-4 my-4 row align-items-center">
        <div class="col-4">
            <img class="img-fluid" :src="celular.imagen" alt="imagen celular">
        </div>
        <div class="col-8">
            <h3 class="text-black fs-4 fw-bold text-uppercase">{{ celular.nombre }}</h3>
            <p>{{ celular.descripcion }}</p>
            <p class="fw-black text-primary fs-3">{{ `$ ${celular.precio}` }}</p>
            <!-- Quitar filtro si no está definido -->
            <button style="border-radius: 15px;" type="button" class="btn btn-dark w-100 ">Agregar al Carrito</button>
        </div>
    </div><!-- FIN CELULAR -->
</template>

<script>
export default {
    props: {
        celular: {
            type: Object,
            required: true
        }
    }
}
</script>

<style lang="scss" scoped></style>