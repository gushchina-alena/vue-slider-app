<template>
    <div class="header">
        <img src="../assets/logo.svg" />
        <div src="controls">
            <a href="#">Кейсы</a>
            <a href="#">Бизнесу</a>
            <a href="#">Услуги</a>
            <a href="#">Контакты</a>
            <!-- <button>Заказать звонок</button> -->
            <Button text="Заказать звонок"></Button>
        </div>
    </div>
</template>

<script>
    import Button from "./Button.vue";
    export default {
        name: "Header",
        components: { Button }
    }
</script>

<style scoped>
.header {
    height: 107px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    box-shadow: 0px 4px 21px rgba(0, 0, 0, 0.07);
    padding-left: 80px;
    padding-right: 80px;
}

a {
    text-decoration: none;
    text-transform: uppercase;
    color: inherit;
    font-size: 16px;
    padding-left: 50px;
}

a:nth-child(2)::before {
    content: url(../assets/star.svg);
    padding-right: 5px;
}

a:hover {
    color: #00A76B;
    cursor: pointer;
}
</style>
