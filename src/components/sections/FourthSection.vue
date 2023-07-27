<script>

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
    created() {
        console.log(this.getImagePath())
    },
    setup() {
        const swiperTextBase = ref( [

            {
                img: 'img/course-02-480x298.jpg',
                price: '$40.00',
                description: 'Learning to Write as a Professional Author',
                numberLessons: '20 lessons',
                students: '50 students'
            },
            {
                img: 'img/stock-full-hd-03-480x298.jpg',
                price: '$0.00 FREE!',
                description: 'Customer-Centric Info-Tech Strategies',
                numberLessons: '24 lessons',
                students: '769 students'
            },
            {
                img: 'img/stock-full-hd-04-480x298.jpg',
                price: '$19.00',
                description: 'Open programming Courses for Everyone: Python',
                numberLessons: '17 lessons',
                students: '62 students'
            },

        ]);
        return {modules: [Pagination, Autoplay], swiperTextBase}
    },
    methods: {
        getImagePath: function(img) {
            return new URL(`../../assets/${img}`, import.meta.url).href;
        }
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
                            <img :src="getImagePath(text.img)" alt="image">

                            <div class="text-card">
                                <h2>{{ text.description }}</h2>
                                <div class="bordo"></div>
                                <p>{{ text.price }}</p>
                                <p> 
                                    <i class="fa-regular fa-file-lines"></i>
                                    {{ text.numberLessons }}
                                </p>
                                <p>
                                    <i class="fa-regular fa-user"></i>
                                    {{ text.students }}
                                </p>
                            </div>

                        </div>

                    </swiper-slide>

                </swiper>

            </div>

        </div>

    </div>

    <div class="under-carousel">

        <p>
            Control your personal preference settings to get notified about
        </p>

        <p>
            appropriate courses. 
            <span>
                View all courses &RightArrow;
            </span>
        </p>

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
        margin-top: 60px;
        transition: all 0.8s ease-in-out;

        &:hover {
        -webkit-box-shadow: -10px 0px 13px -7px #000000, 10px 0px 13px -7px #000000, -50px -50px 0px -30px rgba(0,0,0,0); 
        box-shadow: -10px 0px 13px -7px #000000, 10px 0px 13px -7px #000000, -50px -50px 0px -30px rgba(0,0,0,0);

        }
        border-radius: 5px;
        img {
            border-radius: 5px;
        }
        .card {
            display: flex;
            .text-card {
                text-align: center;
                padding-top: 20px;

                .bordo {
                    border: 2px solid $font-color-secondary;
                    width: 200px;
                    margin-left: 160px;
                    margin-top: 20px;
                    border-radius: 10px;
                }

                h2 {
                    font-size: 1.9rem;
                }

                & p:first-of-type {
                    font-weight: bold;
                    font-size: 1.3rem;
                    color: $background-button;
                    margin-top: 20px;
                }

                & p:nth-of-type(2), p:nth-of-type(3) {
                    font-size: 0.9rem;;
                    color: rgb(133, 133, 133);
                    margin-top: 20px;

                    i {
                        font-size: 0.9rem;
                        margin-right: 5px;
                    }
                }
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

    .under-carousel {
        text-align: center;
        margin-top: 40px;
        padding-bottom: 20px;

        & p {
            color: rgb(133, 133, 133);
        }

        span {
            font-weight: bold;
            color: black;
        }
    }
</style>
