<script>
export default {
	name: "SixthSection",
	components: {

	},
	data() {
		return {

		}
	},
	methods: {
	
		}

}
</script>

<template>
  
    <div class="container-medium">

        <div class="third-section-row">

            <div class="video-col">
                
                <img class="testimonial" src="../../assets/img/home-3-team-image.png" alt="">
                <img class="decoration-over" src="../../assets/img/maxcoach-shape-05-150x150.png" alt="">
                <img class="decoration-over-2" src="../../assets/img/maxcoach-shape-07-150x150.png" alt="">

            </div>

            <div class="text-col">
                
                <p>
                EVERYTHING IN <strong>MAXCOACH</strong>
                </p>

                <h2>We're Here To <span>Transform</span> You!</h2>

                <p>
                    As learners, people can enjoy great companionship from
                    MaxCoach mentors and educators. We can hel you
                    develop and grow at your best.
                </p>

                <button>
                    Get free guide 
                </button>

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
        .third-section-row {
            display: flex;
            justify-content: space-between;
            .video-col {
                width: 60%;
                position: relative;
                .testimonial {
                    position: absolute;
                    top: -77px;
                    left: -8px;
                    width: 437px;
                    z-index: 2;
                }
                .decoration-over {
                    position: absolute;
                    top: 15px;
                    left: -52px;
                    z-index: 1;
                }
                .decoration-over-2 {
                    position: absolute;
                    top: 118px;
                    left: 289px;
                    z-index: 1;
                    width: 132px;
                }
            }
            .text-col {
                width: 40%;
                margin-left: 110px;

                & p:first-of-type {
                font-size: 0.8rem;
                color: rgb(133, 133, 133);
                }

                & p:nth-of-type(2) {
                font-size: 0.8rem;
                color: rgb(133, 133, 133);
                padding-right: 10px;
                text-align: justify;
                margin-top: 10px;
                }

                & p:nth-of-type(3) {
                font-size: 0.8rem;
                color: black;
                margin-top: 10px;
                font-weight: bold;
                }

                h2 {
                font-size: 2.9rem;
                font-weight: 400;
                margin-top: 20px;

                    span {
                        color: $background-button;
                    }
                }

                button {
                    margin-top: 30px;
                    border: none;
                    background-color: $background-button;
                    color: white;
                    padding: 15px 25px;
                    border-radius: 5px;
                    font-weight: bold;
                    cursor: pointer;
                }
            }
        }
</style>
