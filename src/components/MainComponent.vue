<script>

export default {
	name: "MainComponent",
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
  
    <main>

		<div class="jumbo-section">

			<h3>Commence Business</h3>

			<h1>Distant Mentoring Program</h1>

			<button>Download free guidebook ++></button>

		</div>
		
		<div class="second-section">

			<div class="container-medium">

				<div class="second-section-main">

					<div class="learn-about">

						<p>EVERYTHING IN MAXCOACH</p>

						<h2>Learn about our Work  Culture at Maxcoach</h2>

						<p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quibusdam, excepturi.</p>

						<p>Have questions? Get free guide</p>

					</div>

					<div class="learn-about-image">

						IMAGE

					</div>

				</div>

			</div>			

			<div class="second-section-foot">

				<div class="container-small">

					<div class="score-recap">

						<div class="enrolleds">

							<p>129+</p>
							<p>ENROLLLED LEARNS</p>
							
						</div>

						<div class="sessions">

							<p>80</p>
							<p>FINISHED SESSIONS</p>

						</div>

						<div class="satisfaction-rate">

							<p>4%</p>
							<p>SATISFACTION RATE</p>

						</div>

					</div>

				</div>

			</div>

		</div>

		<div class="third-section">

			<div class="container-medium">

				<div class="third-section-row">

					<div class="video-col">
						
						IMAGE

					</div>

					<div class="text-col">
						
						<p>HOW WE WORK</p>

						<h2>Upgrade your Skills Upgrade Your Life</h2>

						<p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ex, necessitatibus.</p>

						<p>Download free guidebook</p>

					</div>

				</div>
			
			</div>

		</div>

    </main>

</template>

<style lang="scss" scoped>
	.jumbo-section {
		text-align: center;
	}
	.container-medium {
		max-width: 1000px;
		margin: 0 auto;
		padding: 0;
	}
	.container-small {
		max-width: 800px;
		margin: 0 auto;
		padding: 0;
	}
	.second-section {
		padding-top: 40px;
		.second-section-main {
			display: flex;
			justify-content: space-between;
		}
		.score-recap {
			display: flex;
			justify-content: space-between;
			margin-top: 20px;

			.enrolleds, .sessions, 
			.satisfaction-rate p {
				text-align: center;
			}
		}
	}
	.third-section {
		padding-top: 40px;
		.third-section-row {
			display: flex;
			justify-content: space-between;
		}
	}
</style>
