<script>
import imgOne from "../../assets/img/course-02-480x298.jpg"

import {Swiper, SwiperSlide} from 'swiper/vue'
import {Autoplay, Pagination} from 'swiper/modules'

import 'swiper/css';
import 'swiper/css/pagination';

import { ref } from 'vue';

export default {
	name: "FourthSection.vue",
    components: {
        Swiper,
        SwiperSlide
    },
    setup() {
        const swiperTextBase = ref( [
            {
                imgOne,
                price: '$40.00',
                description: 'Learning to Write as a Professional Author',
                numberLessons: '20',
                students: '50'
            },
            {
                imgOne,
                price: '$40.00',
                description: 'ciao ciao ciao',
                numberLessons: '20',
                students: '50'
            },
            {
                imgOne,
                price: '$40.00',
                description: 'ciao ciao ciao',
                numberLessons: '20',
                students: '50'
            },

        ]);
        return {modules: [Pagination, Autoplay], swiperTextBase}
    }
}
</script>

<template>
    <div class="title-fourth-section">

        <p>
            JOIN MAXCOACH AT THE BEST
        </p>

        <h2>
            Latest Online <span>Courses</span>
        </h2>
    
    </div>

    <div class="container-medium">
        <div class="carousel-contain">
            <div class="col-carousel">
                <swiper
                    :modules="modules"
                    :space-between="20"
                    :loop="true"
                    :pagination="{clickable: true}"
                    :autoplay="{
                        delay: 7000,
                        disableOnInteraction: false,
                        pauseOneMouseEnter:true
                    }"
                >
                    <swiper-slide v-for="text in swiperTextBase" :key="text.description">

                        <div class="card">
                            <img :src="text.imgOne" alt="image">

                            <div class="text-card">
                                <h1>{{ text.author }}</h1>
                                <p>{{ text.description }}</p>
                                <p>{{ text.price }}</p>
                            </div>

                        </div>

                    </swiper-slide>

                </swiper>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use "../../assets/scss/partials/variables.scss" as *;
    .container-medium {
		max-width: 1000px;
		margin: 0 auto;
		padding: 0;
	}

    .carousel-contain {
        padding-top: 80px;
        img {
            width: 500px;
            border-radius: 5px;
        }
        .card {
            display: flex;
            .text-card {
                text-align: right;
                padding-left: 214px;
            }
        }
    }
    .title-fourth-section {
        text-align: center;

        & p:first-of-type {
            font-size: 0.8rem;
            color: rgb(133, 133, 133);
        }
        h2 {
            font-size: 2.9rem;
            font-weight: 400;
            margin-top: 20px;

            span {
                color: $background-button;
            }
        }
    }
</style>
