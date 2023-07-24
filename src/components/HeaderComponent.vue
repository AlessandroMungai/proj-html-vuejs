<script>
export default {
	name: "HeaderComponent",
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
  
    <header>

		<div class="nav-row">

			<div class="nav-menu">
				<ul>
					<li>
						<a href="#">Home <i class="fa-solid fa-angle-down"></i></a>
					</li>
					<li>
						<a href="#">Pages <i class="fa-solid fa-angle-down"></i></a>
					</li>
					<li>
						<a href="#">Courses <i class="fa-solid fa-angle-down"></i></a>
					</li>
					<li>
						<a href="#">Features <i class="fa-solid fa-angle-down"></i></a>
					</li>
					<li>
						<a href="#">Blog <i class="fa-solid fa-angle-down"></i></a>
					</li>
					<li>
						<a href="#">Shop <i class="fa-solid fa-angle-down"></i></a>
					</li>
				</ul>
			</div>

			<div class="nav-logo">
				<img src="../assets/img/dark-logo.png" alt="logo">
			</div>

			<div class="nav-search">
				SEARCH BUTTON
			</div>

		</div>

    </header>

</template>

<style lang="scss" scoped>
	.nav-row {
	display: flex;
	justify-content: space-between;
	padding: 40px;
	}

	ul {
		display: flex;
		list-style-type: none;

		li {
			
			a {
				text-decoration: none;
				color: black;
				padding-right: 30px;
				font-size: 1rem;
			}
		}
	}
	.nav-menu {
		width: 40%;
	}
	.nav-logo {
		width: 20%;
		text-align: center;

		img {
			width: 130px;
			margin-left: 10px;
		}
	}
	.nav-search {
		width: 40%;
		text-align: right;
	}

</style>
