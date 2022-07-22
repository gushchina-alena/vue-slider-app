<template>
    <div class="services">
        <h2>Наши услуги</h2>
        <div class="services__cards">
            <template v-if="allImagesPrinted">
                <Card v-for="(card, id) in cardImages"
                    :card="card"
                />
            </template>
            <template v-else>
                <Card v-for="(card, id) in printSix"
                    :card="card"
                />
            </template>
        </div>
        <div class="services__btn">
            <button v-on:click="onShowAllClick" :class="{ invisible: allImagesPrinted }">Все услуги</button>
        </div>
    </div>
</template>

<script>
    import Card from "./Card.vue"; 
    import card1 from "../../assets/services-pic1.jpg";
    import card2 from "../../assets/services-pic2.jpg";
    import card3 from "../../assets/services-pic3.jpg";
    import card4 from "../../assets/services-pic4.jpg";
    import card5 from "../../assets/services-pic5.jpg";
    import card6 from "../../assets/services-pic6.jpg";
    import card7 from "../../assets/services-pic4.jpg";
    import card8 from "../../assets/services-pic5.jpg";
    import card9 from "../../assets/services-pic6.jpg";

    export default { 
        components: { Card },
        data: () => ({
            cardImages: [card1, card2, card3, card4, card5, card6, card7, card8, card9],
            allImagesPrinted: false
        }),
        methods: {
            onShowAllClick: function () {
                this.allImagesPrinted = true;
            }
        },
        computed: {
            printSix: function () {
                return this.cardImages.slice(0, 6);
            }
        }
        
    }
</script>

<style scoped>
h2 {
    font-size: 40px;
    padding-top: 40px;
}
.services {
    width: 75%;
    margin: 0 auto;
}
.services__cards {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    justify-content: center;
}

.services__btn {
    width: 100%;
    text-align: center;
    padding-top: 10px;
    padding-bottom: 40px;
}

button {
    width: 200px;
    height: 49px;
    color: #00A76B;
    background-color: transparent; 
    border: 1.5px solid #00BB78;
    border-radius: 30px;
    font-size: 18px;
    cursor: pointer;
}

.invisible {
    display: none;
}

@media all and (max-width: 1880px) {
    h2 {
        text-align: center;
    }
    .services {
        width: 84%;
    }
}

@media all and (max-width: 1690px) {
    .services {
        width: 100%;
    }
}

@media all and (max-width: 1690px) {
    .services {
        width: 100%;
    }
}

@media all and (max-width: 1400px) {
    h2 {
        font-size: 30px;
    }
}

@media all and (max-width: 800px) {
    h2 {
        font-size: 26px;
    }
}

</style>
