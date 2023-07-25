<script>
import NavComponent from '../components/NavComponent.vue';

export default {
	name: "HeaderComponent",
	components: {
		NavComponent
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
  
    <header>

		<div class="nav-row">

			<div class="nav-menu">

				<NavComponent />

			</div>

			<div class="nav-logo">
				<img src="../assets/img/dark-logo.png" alt="logo">
			</div>

			<div class="nav-search">

				<div class="search-contain">

					<i class="fa-solid fa-cart-shopping cart-icon">
						<span>
							0
						</span>
					</i>
					
					<i class="fa-regular fa-circle-user"></i>

					<div class="input-section">

						<input type="text" placeholder="Search...">

						<i class="fa-solid fa-magnifying-glass"></i>

					</div>

				</div>

			</div>

		</div>

    </header>

</template>

<style lang="scss" scoped>
	@use "../assets/scss/partials/variables.scss" as *;
	.nav-row {
	display: flex;
	justify-content: space-between;
	padding: 20px;
	align-items: center;

	}
	.nav-menu {
		width: 45%;
		padding-left: 50px;
		position: relative;
	}
	.nav-logo {
		width: 10%;
		text-align: center;

		img {
			width: 150px;
			margin-left: 10px;
		}
	}
	.nav-search {
		width: 45%;
		padding-right: 50px;
		.search-contain {
			display: flex;
			justify-content: end;
			align-items: center;

			& i {
				margin-right: 30px;
				font-size: larger;
			}
			.input-section {
				position: relative;
				font-size: large;

				& i {
					position: absolute;
					top: 10px;
					right: -19px;
					color: $background-button;
				}

				input {
					padding: 10px;
					background-color: rgb(237, 237, 237);
					border: none;
					border-radius: 5px;
				}
			}
			.cart-icon {
				position: relative;
				span {
					position: absolute;
					top: -11px;
					font-size: small;
					background-color: $background-button;
					width: 20px;
					height: 20px;
					border-radius: 50%;
					padding: 5px;
					color: white;
					line-height: 10px;
					text-align: center;
				}
			}
		}

	}

</style>
