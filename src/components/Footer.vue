<template>
    <footer>
        <nav>
            <img class="footer-pic" src="../assets/footer-pic.png" />
            <div class="nav-block contact">
                <h3>Для связи</h3>
                <div class="tel-block">
                    <img src="../assets/footer-icon1.svg" /> 
                    <a href="tel:+74951234567">7 (926) 126-64-57</a>
                </div>
                <div class="tel-block">
                    <img src="../assets/footer-icon2.svg" /> 
                    <a href="tel:+74951234567">7 (926) 126-64-57</a>
                </div>
                <div class="tel-block">
                    <img src="../assets/footer-icon3.svg" /> 
                    <a href="tel:+74951234567">7 (926) 126-64-57</a>
                </div>
            </div>
            <div class="nav-block company">
                <h3>Компания</h3>
                <a href="#">Услуги</a>
                <a href="#">Кейсы</a>
                <a href="#">Контакты</a>
                <a href="#">Сотрудничество</a>
            </div>
            <div class="nav-block documents">
                <h3>Документы</h3>
                <a href="#">Политика конфеденциальности</a>
                <a href="#">Пользовательское соглашение</a>
            </div>
            <div class="newsletter">
                <h3>Будьте в курсе</h3>
                <div class="newsletter-input">
                    <input placeholder="E ‒ mail" />
                    <img class="send-btn" src="../assets/send.svg" />
                </div>
                <div class="newsletter-icons">
                    <img src="../assets/footer-icon4.svg" />
                    <img src="../assets/footer-icon5.svg" />
                    <img src="../assets/footer-icon6.svg" />
                </div>
            </div>
        </nav>
        <p class="copyright">Copyright © 2022 SCID</p>
    </footer>
</template>

<script>

</script>

<style scoped>
footer {
    box-sizing: border-box;
    height: 366px;
    padding: 40px;
    padding-bottom: 10px;
    width: 100%;
    background-color: #00A76B;
}

.footer-pic {
    padding-top: 35px;
}

nav {
    height: 270px;
    display: flex;
    align-items: flex-start;
    justify-content: space-around;
}

.nav-block {
    display: flex;
    flex-direction: column;
}

.tel-block {
    display: flex;
    align-items: center;
    padding-bottom: 20px;
}

.tel-block a {
    padding-left: 10px;
}

a {
    display: block;
    text-decoration: none;
    color: #fff;
    font-size: 16px;
}

.contact a {
    font-size: 14px;
}

.company a, 
.documents a {
    padding-bottom: 15px;
}

.documents {
    width: 10%;
}

h3 {
    color: #fff;
    font-weight: 500;
    font-size: 20px;
    margin-bottom: 24px;
}

input {
    padding-left: 12px;
    color: #fff;
    width: 255px;
    height: 40px;
    background-color: #33b989;
    border-radius: 8px;
    border: none;
    outline: none;
}

input::placeholder {
    color: inherit;
    opacity: none;
}

.newsletter-input {
    position: relative;
}

.send-btn {
    position: absolute;
    right: 11px;
    top: 11px;
    cursor: pointer;
}

.newsletter-icons {
    display: flex;
    align-items: center;
    padding-top: 50px;
}

.newsletter-icons img {
    padding-right: 16px;
    cursor: pointer;
}

.copyright {
    text-align: center;
    font-family: inherit;
    font-size: 14px;
    color: #fff;
}
</style>
