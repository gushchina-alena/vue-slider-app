<template>
    <div class="carousel">
        <div class="carousel-inner">
            <CarouselItem
                v-for="(slide, index) in slides"
                :slide="slide"
                :key="`item-${index}`"
                :current-slide="currentSlide"
                :index="index"
            >
            </CarouselItem>
            <div class="controls">
                <button v-on:click="onSliderClick(id)" 
                v-for="(btn, id) in slides.length"
                :class="{ active: currentSlide === id }"
            ></button>
            </div>
            
            <!-- <CarouselControls :index="index" :current-slide="currentSlide"></CarouselControls> -->
        </div>
    </div>
</template>

<script>
import CarouselItem from "./CarouselItem";
import CarouselControls from "./CarouselControls.vue";

    export default {
        props: ["slides"],
        components: { CarouselItem },
        data: () => ({
            currentSlide: 0,
        }),
        methods: {
            onSliderClick: function (id) {
                this.currentSlide = id; 
            }
        }
    }
</script>

<style scoped>
button {
    width: 20px;
    height: 20px;
    background-color: #E2E3E5;
    border-radius: 80%;
    border: none;
    margin: 0 10px;
    cursor: pointer;
}

button:hover,
.active {
    background-color: #00BB78;
}

.controls {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 20px;
}
</style>