<script>
export default {
	name: "SeventhSection",
	components: {

	},
	data() {
		return {
            cards: [

                {
                    img: 'img/artist-blog-03-480x325.jpeg',
                    job: 'ARTIST',
                    title: 'Brush Strokes Energize Trees in Paintings',
                    date: 'May, 15,2020',
                    views: '688'
                },
                {
                    img: 'img/artist-blog-01-480x325.jpg',
                    job: 'ARTIST',
                    title: 'Poked-Sized Notebooks Hold Miniature Paintings',
                    date: 'May, 15,2020',
                    views: '603'
                },
                {
                    img: 'img/artist-blog-02-480x325.jpg',
                    job: 'ARTIST',
                    title: 'Connection Between Self-Portaits and Identity',
                    date: 'May, 15,2020',
                    views: '397'
                },

            ]
		}
	},
	methods: {
        getImagePath: function(img) {
            return new URL(`../../assets/${img}`, import.meta.url).href;
        }
	}

}
</script>

<template>
  
    <div class="container-medium">
        
        <p class="first-p">
            READ FOR MORE JOYMENT
        </p>

        <h2>Latest From <span>Oure Blogs</span></h2>

        <div class="blog-contain">

            <div class="blog-cards">

                <div class="singlecard" v-for="(card, index) in cards" :key="index">

                    <img :src="getImagePath(card.img)" :alt="card.title">

                    <p> {{ card.job }} </p>

                    <h3>{{ card.title }}</h3>

                    <span> {{ card.date }}</span>

                    <span> {{ card.views }}</span>

                </div>

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
            .first-p {
                font-size: 0.8rem;
                color: rgb(133, 133, 133);
                text-align: center;
                padding-top: 75px;
            }
        }

        h2 {
            font-size: 2.9rem;
            font-weight: 400;
            margin-top: 20px;
            text-align: center;

            span {
                color: $background-button;
            }
        }
        .blog-contain {
            margin-top: 40px;
            .blog-cards {
                display: flex;
                justify-content: space-between;
                .singlecard {
                    width: calc(100% / 3 - 20px);
                    height: 400px;
                    margin: 0 10px;
                    transition: all 1s ease-in-out;

                    &:hover {
                        transform: scale(1.1);
                    }

                    p {
                        text-align: left;
                        margin-top: 15px;
                        color: rgb(133, 133, 133);
                    }

                    h3 {
                        margin-top: 15px;
                        margin-bottom: 15px;
                    }

                    span {
                        font-size: 0.8rem;
                        color: rgb(133, 133, 133);
                        margin-right: 20px;
                        margin-top: 15px;
                        padding-bottom: 75px;
                    }

                    img {
                        width: 100%;
                        border-radius: 10px;
                    }
                }
            }

        }

</style>
