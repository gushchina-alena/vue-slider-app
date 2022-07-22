<template>
    <header class="header">
        <img src="../assets/logo.svg" alt="App logo" />
        <div src="header__controls">
            <a href="#">Кейсы</a>
            <a href="#">Бизнесу</a>
            <a href="#">Услуги</a>
            <a href="#">Контакты</a>
            <button>Заказать звонок</button>
        </div>
    </header>
</template>

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

@media all and (max-width: 950px) {
    .header { 
        height: 300px;
        flex-direction: column;
        justify-content: flex-start;
    }

    .header img {
        width: 80px;
        height: 80px;
        padding-top: 20px;
        padding-bottom: 10px;
    }

    a {
        display: block;
        padding-left: 0;
        padding-bottom: 10px;
        text-align: center;
    }

    a:nth-child(2)::before {
        content: none;
    }

    button {
        margin-left: 0;
        width: 180px;
        height: 45px;
        font-size: 16px;
    }
}
</style>
