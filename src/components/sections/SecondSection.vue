<script>
export default {
	name: "SecondSection",
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

    <div class="second-section-main">

        <div class="learn-about">

            <p>EVERYTHING IN <strong>MAXCOACH</strong></p>

            <h2>Learn about our <span>Work  Culture</span> at Maxcoach</h2>

            <p>
                Spend some time to visit our website or head office and discover our current courses,
                enorollment procedure, and registration deadline. We're opening new classes every beginning
                of each month.
            </p>

            <p>Have questions? <span>Get free guide &RightArrow;</span></p>

        </div>

        <div class="learn-about-image">
            
            <img class="img-under" src="../../assets/img/maxcoach-shape-07-150x150.png" alt="">

            <img class="img-principal" src="../../assets/img/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="">

            <img class="img-over" src="../../assets/img/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg" alt="">
        
            <img class="img-over-2" src="../../assets/img/maxcoach-shape-02.png" alt="">
            
        </div>

    </div>
	
    <div class="second-section-foot">

        <div class="container-small">

            <div class="score-recap">

                <div class="enrolleds">

                    <h4>129+</h4>
                    <p>ENROLLLED LEARNS</p>
                    
                </div>

                <div class="sessions">

                    <h4>80</h4>
                    <p>FINISHED SESSIONS</p>

                </div>

                <div class="satisfaction-rate">

                    <h4>4%</h4>
                    <p>SATISFACTION RATE</p>

                </div>

            </div>

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
    .second-section-main {
        display: flex;
        justify-content: space-between;

        .learn-about {
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
                color: rgb(133, 133, 133);
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
                z-index: 2;
            }
            .img-over {
                position: absolute;
                top: -81px;
                right: -86px;
                border-radius: 5px;
                z-index: 3;
            }
            .img-over-2 {
                width: 120px;
                position: absolute;
                top: 314px;
                right: 48px;
                border-radius: 5px;
                z-index: 3;
            }
            .img-under {
                position: absolute;
                top: -41px;
                right: 62px;
                z-index: 1;
                clip-path: inset(0 0 70% 0);
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
