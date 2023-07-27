<script>
export default {
	name: "EightSection",
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

    <div class="form">

        <h2>
            Subscrive <span>Newsletter</span>
        </h2>

        <p>
            Enter your mail address to register to our newsletter subscription
            delivered on a regular basis!
        </p>
        <div class="input-section">

            <input type="text" placeholder="Enter your email">

            <button>
                Subscrive
            </button>

        </div>

        <img class="circle-decoration" src="../../assets/img/maxcoach-shape-01.png" alt="">

    </div>

</template>

<style lang="scss" scoped>
    @use "../../assets/scss/partials/variables.scss" as *;
    .form {
        display: flex;
        flex-direction: column;
        align-items: center;
        position: relative;
        h2 {
            font-size: 2.9rem;
            font-weight: 400;
            margin-top: 20px;

            span {
                color: $background-button;
            }
        }
        p {
            color: rgb(133, 133, 133);
            margin-top: 20px;
            font-weight: bold;
        }
        .input-section {
            display: flex;
            height: 20px;
            align-items: center;
            margin-top: 40px;
            margin-bottom: 50px;

            input {
                border: none;
                background-color: #EDEDED;
                padding: 10px 40px;
                text-align: left;
                vertical-align: middle;
                border-bottom-left-radius: 5px;
                border-top-left-radius: 5px;
            }

            button {
                vertical-align: middle;
                padding: 10px 20px;
                border: none;
                background-color: $background-button;
                color: white;
                border-top-right-radius: 5px;
                border-bottom-right-radius: 5px;
            }
        }
        .circle-decoration {
            position: absolute;
            right: 720px;
            top: -66px;
            width: 101px;
        }
    }

</style>
