<template>
    <footer class="footer">
        <nav class="footer__nav">
            <img class="footer__img" src="../assets/footer-pic.png" />
            <div class="nav-block nav-block_contact">
                <h3>Для связи</h3>
                <div class="nav-block__tel">
                    <img src="../assets/footer-icon1.svg" /> 
                    <a href="tel:+74951234567">7 (926) 126-64-57</a>
                </div>
                <div class="nav-block__tel">
                    <img src="../assets/footer-icon2.svg" /> 
                    <a href="tel:+74951234567">7 (926) 126-64-57</a>
                </div>
                <div class="nav-block__tel">
                    <img src="../assets/footer-icon3.svg" /> 
                    <a href="tel:+74951234567">7 (926) 126-64-57</a>
                </div>
            </div>
            <div class="nav-block nav-block_company">
                <h3>Компания</h3>
                <a href="#">Услуги</a>
                <a href="#">Кейсы</a>
                <a href="#">Контакты</a>
                <a href="#">Сотрудничество</a>
            </div>
            <div class="nav-block nav-block_documents">
                <h3>Документы</h3>
                <a href="#">Политика конфеденциальности</a>
                <a href="#">Пользовательское соглашение</a>
            </div>
            <div class="footer__newsletter">
                <h3>Будьте в курсе</h3>
                <div class="input">
                    <input placeholder="E ‒ mail" />
                    <img class="input__btn" src="../assets/send.svg" />
                </div>
                <div class="footer__icons">
                    <img src="../assets/footer-icon4.svg" />
                    <img src="../assets/footer-icon5.svg" />
                    <img src="../assets/footer-icon6.svg" />
                </div>
            </div>
        </nav>
        <p class="footer__copyright">Copyright © 2022 SCID</p>
    </footer>
</template>

<style scoped>
.footer {
    box-sizing: border-box;
    height: 366px;
    padding: 40px;
    padding-bottom: 10px;
    width: 100%;
    background-color: #00A76B;
}

.footer__img {
    padding-top: 35px;
}

.footer__nav {
    height: 270px;
    display: flex;
    align-items: flex-start;
    justify-content: space-around;
}

.nav-block {
    display: flex;
    flex-direction: column;
}

.nav-block__tel {
    display: flex;
    align-items: center;
    padding-bottom: 20px;
}

.nav-block__tel a {
    padding-left: 10px;
}

a {
    display: block;
    text-decoration: none;
    color: #fff;
    font-size: 16px;
}

.nav-block_contact a {
    font-size: 14px;
}

.nav-block_company a, 
.nav-block_documents a {
    padding-bottom: 15px;
}

.nav-block_documents {
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

.input {
    position: relative;
}

.input__btn {
    position: absolute;
    right: 11px;
    top: 11px;
    cursor: pointer;
}

.footer__icons {
    display: flex;
    align-items: center;
    padding-top: 50px;
}

.footer__icons img {
    padding-right: 16px;
    cursor: pointer;
}
.footer__copyright {
    text-align: center;
    font-family: inherit;
    font-size: 14px;
    color: #fff;
}

@media all and (max-width: 1350px) {
    .footer {
        padding-left: 20px;
        padding-right: 20px;
    }

    .footer__nav {
        flex-wrap: wrap;
    }
    .footer__img {
        display: none;
    }

    input {
        width: 200px;
    }
}

@media all and (max-width: 1100px) {
    .footer {
        height: fit-content;
        padding-top: 20px;
    }

    .footer__nav {
        height: fit-content;
        flex-direction: column;
        align-items: center;
        text-align: center;
    }

    .nav-block_documents {
        display: none;
    }

    input {
        width: 180px;
    }

    .footer__icons {
        padding-top: 20px;
        padding-bottom: 10px;
        justify-content: center;
    }
}
</style>
