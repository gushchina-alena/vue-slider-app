<template>
    <div class="card">
        <img :src="card" />
        <p>Кадастровые работы в отношении земельных участков</p>
    </div>
</template>

<script>
    export default {
        props: ["card"],
    }
</script>

<style scoped>
.card {
    width: 411px;
    height: 383px;
    box-shadow: 0px 4px 20px rgba(0, 0, 0, 0.06);
    border-radius: 20px;
    margin: 30px 30px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
}
p {
    font-size: 20px;
    font-weight: 600;
    width: 363px;
    color: #000;
    cursor: pointer;
}
p:hover {
    color: #00BB78;
}
</style>
