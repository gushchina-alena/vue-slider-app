<template>
    <button>{{text}}</button>
</template>

<script>
    export default {
        props: ["text"],
    }
</script>

<style scoped>
button {
    width: 200px;
    height: 49px;
    margin-left: 50px;
    color: #00A76B;
    background-color: transparent; 
    border: 1.5px solid #00BB78;
    border-radius: 30px;
    font-size: 18px;
    cursor: pointer;
}
</style>
