<script>
export default {
	name: "FooterComponent",
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
  
    <div class="jumbo-section">

        <div class="text-jumbo">

            <h3>Commence Business</h3>

            <h1>Distant Mentoring Program</h1>

            <button>
                Download free guidebook &RightArrow;
            </button>

        </div>

        <div class="aside-icon">

            <i class="fa-solid fa-ruler-combined"></i>
            <i class="fa-regular fa-life-ring"></i>
            <i class="fa-solid fa-book"></i>
            <i class="fa-solid fa-cart-shopping"></i>

        </div>

    </div>

</template>

<style lang="scss" scoped>
    @use "../../assets/scss/partials/variables.scss" as *;
	.jumbo-section {
		height: 700px;
		text-align: center;
		background-image: url(../../assets/img/home-3-hero-bg.jpg);
		display: flex;
		justify-content: center;
		align-items: center;
		position: relative;
		.text-jumbo {
			h3 {
				font-size: 2.4rem;
				color: white;
			}
			h1 {
				font-size: 3.6rem;
				color: white;
				font-weight: 400;
			}
			button {
				margin-top: 30px;
				border: none;
				background-color: white;
				color: $background-button;
				padding: 15px 25px;
				border-radius: 5px;
				font-weight: bold;

				&:hover {
					background-color: $background-button;
					color: white;	
				}
			}
		}
		.aside-icon {
			display: flex;
			flex-direction: column;
			justify-content: center;
			align-items: center;
			background-color: white;
			position: absolute;
			right: 0;
			padding-top: 20px;
			padding-left: 10px;
			padding-right: 10px;
			border-radius: 5px;

			i {
				margin-bottom: 20px;
				color: rgb(101, 101, 101);
				cursor: pointer;

				&:hover {
					color: $background-button;
				}
			}

		}
	}    
</style>
