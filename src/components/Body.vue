<template>
    <div class="Body">
            <p>Hola</p>
            <div class="boton">
            <button class="btn btn-danger">+</button>
            </div>
            <Menu></Menu>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.Body{
display: flex;
width: 1440px;
height: 1024px;
background: #FFFFFF;
}
.boton{
    display: flex;
    justify-content: flex-start;
    flex-direction: column-reverse;

    height: 100px;
}

</style>