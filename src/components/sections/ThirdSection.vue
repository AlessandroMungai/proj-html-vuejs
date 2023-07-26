<script>
export default {
	name: "ThirdSection",
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
                
                <img class="youtube-image" src="../../assets/img/stock-full-hd-11-670x450.jpg" alt="">

                <img class="youtube-icon" src="../../assets/img/icon-youtube-play.png" alt="">

                <img class="circle-under" src="../../assets/img/maxcoach-shape-05.png" alt="">

                <img class="quarter-under" src="../../assets/img/maxcoach-shape-07-150x150.png" alt="">

            </div>

            <div class="text-col">
                
                <p>HOW WE WORK</p>

                <h2>Upgrade your Skills <span>Upgrade Your Life</span></h2>

                <p>
                    Opening up more opportunities in front of you to get the ticket
                    to more enjoyable door in life. Getting equipped with new skills
                    for new sets of insights into your career.
                    MaxCoach accompany learners in every stage of learning
                </p>

                <p>Download free guidebook &RightArrow;</p>

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
            .youtube-image {
                width: 100%;
                position: relative;
                z-index: 2;
            }
            .youtube-icon {
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
                width: 50px;
                z-index: 3;
            }
            .circle-under {
                width: 120px;
                position: absolute;
                top: -40px;
                left: -45px;
                z-index: 1;
            }
            .quarter-under {
                width: 100px;
                position: absolute;
                bottom: -40px;
                right: -30px;
                z-index: 1;
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
        }
    }
</style>
