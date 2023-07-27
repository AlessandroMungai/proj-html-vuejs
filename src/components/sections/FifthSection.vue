<script>
export default {
	name: "FifthComponent",
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

    <div class="fifth-section-contain">

        <div class="testimonial-about">

            <p>TESTIMONIALS</p>

            <h2>Why Do People<span>*Hearts*</span> Us?</h2>

            <p>
                Seeking for verbals of our service quality? Finde them here.
                Everything is trasparent and straightforward for your sense of justification.
            </p>

            <p>View all &RightArrow;</p>

        </div>

        <div class="learn-about-image">
            
            <img class="img-principal" src="../../assets/img/stock-full-hd-06-480x298.jpg" alt="">

        </div>

    </div>

</div>

</template>

<style lang="scss" scoped>
@use "../../assets/scss/partials/variables.scss" as *;
    .container-small {
		max-width: 600px;
		margin: 0 auto;
		padding: 0;
	}
    .container-medium {
		max-width: 1000px;
		margin: 0 auto;
		padding: 0;
	}
    .fifth-section-contain {
        display: flex;
        justify-content: space-between;
        margin-top: 40px;

        .testimonial-about {
            width: 40%;
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
                font-weight: bold;
                margin-top: 10px;

                span {
                    color: $background-button;
                    text-decoration: underline;
                    cursor: pointer;
                }
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
        .learn-about-image {
            width: 60%;
            position: relative;
            margin-left: 95px;
            .img-principal {
                border-radius: 5px;
                margin-left: 20px;
                z-index: 2;
            }
        }
    }
    .score-recap {
        display: flex;
        justify-content: space-between;
        margin-top: 20px;
        text-align: center;

        h4 {
            font-size: 1.6rem;
            color: $background-button;
            margin-top: 60px;
        }

        p {
            font-size: 0.8rem;
        }
    }

</style>
