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
.carousel-item img {
    width: 100%;
    height: 672px;
    margin-top: 30px;
    position: relative;
}

.carousel-item h1 {
    font-size: 64px;
    width: 790px;
    position: absolute;
    top: 300px;
	left: 100px;
}

h1 span {
    color: #00A76B;
}
</style>
