<template>
    <div
        class="carousel-item"
        v-show="currentSlide === index"
        :slide="slide"
    >
        <img :src="slide" alt="Slider image"/>
        <h1>Lorem ipsum dolor sit amet, <span>consectetur adipiscing elit</span></h1>
    </div>
</template>

<script>
    export default {
        props: ["slide", "currentSlide", "index"],
    }
</script>

<style scoped>
img {
    width: 100%;
    height: 672px;
    margin-top: 30px;
    position: relative;
}

h1 {
    font-size: 64px;
    width: 790px;
    position: absolute;
    top: 300px;
	left: 100px;
}

h1 span {
    color: #00A76B;
}

@media all and (max-width: 1400px) {
    h1 {
        font-size: 54px;
        width: 700px;
    }
}

@media all and (max-width: 1100px) { 
    h1 {
        font-size: 44px;
        width: 460px;
    }
}

@media all and (max-width: 950px) { 
    img {
        height: 500px;
    }

    h1 {
        font-size: 38px;
        width: 400px;
        top: 480px;
    }
}

@media all and (max-width: 700px) { 
    img {
        height: 370px;
    }

    h1 {
        font-size: 30px;
        width: 320px;
        top: 430px;
        left: 60px;
    }
}

@media all and (max-width: 450px) { 
    img {
        height: 300px;
    }

    h1 {
        display: none;
    }
}
</style>
