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
  
	<footer>

		<div class="container-medium">

			<div class="foot-contain">

				<div class="foot-row">

					<div class="foot-col-left">

						<h5>
							Address
						</h5>

						<p>
							382 NE 191st St # 87394 Miami, FL 33179-3899
						</p>

						<p>
							+1(305) 547-9909 (9am - 5pm EST, Monday - Friday)
						</p>

						<p>
							support@maxcoach.com
						</p>

						<div class="icon-foot">
							<i class="fa-brands fa-square-facebook"></i>
							<i class="fa-brands fa-twitter"></i>
							<i class="fa-brands fa-instagram"></i>
							<i class="fa-brands fa-linkedin"></i>
						</div>

					</div>

					<div class="foot-col-right">

						<div class="lists-foot">

							<ul>
								<li>
									<a class="title-list" href="#">
										Explore
									</a>
								</li>
								<li>
									<a href="#">
										Start here
									</a>
								</li>
								<li>
									<a href="#">
										Blog
									</a>
								</li>
								<li>
									<a href="#">
										About us
									</a>
								</li>
							</ul>

							<ul class="second-lists">

								<li>
									<a href="#">
										Success story
									</a>
								</li>
								<li>
									<a href="#">
										Courses
									</a>
								</li>
								<li>
									<a href="#">
										Contact us
									</a>
								</li>
							</ul>

							<ul class="third-lists">

								<li>
									<a class="title-list" href="#">
										Information
									</a>
								</li>
								<li>
									<a href="#">
										Membership
									</a>
								</li>
								<li>
									<a href="#">
										Purchase guide
									</a>
								</li>
								<li>
									<a href="#">
										Privacy policy
									</a>
								</li>
								<li>
									<a href="#">
										Terms of service
									</a>
								</li>
							</ul>

						</div>

					</div>

				</div>

				<p class="copy"> 
					2023 MaxCoach. All Rights Reserved
				</p>
				<a href="#jump-to">
				<i class="fa-solid fa-circle-arrow-up up-to-page"></i>
				</a>
			</div>

		</div>

	</footer>

</template>

<style lang="scss" scoped>
	@use "../assets/scss/partials/variables.scss" as *;

		footer {
			background-color: #171621;
			.container-medium {
				max-width: 1000px;
				margin: 0 auto;
				padding: 0;
			}
			.foot-contain {
				padding-top: 50px;
				position: relative;	
				.foot-row {
					display: flex;
					.foot-col-left {
						width: 60%;
						color: white;

						p {
							color: rgb(133, 133, 133);
							margin-top: 15px;
							font-size: 0.8rem;
						}
						.icon-foot {
							display: flex;
							margin-top: 20px;

							& i {
								margin-right: 20px;
								color: rgb(133, 133, 133);
								font-size: larger;

								&:hover {
									color: $background-button;
								}
							}

						}
					}
					.foot-col-right {
						width: 40%;
						.lists-foot {
							display: flex;

							ul {
								list-style-type: none;

								li {
									margin-bottom: 10px;
									.title-list {
										font-weight: bold;
										color: white;
									}

									a {
										text-decoration: none;
										color: rgb(133, 133, 133);
										font-size: 0.8rem;
									}
								}
							}

							.second-lists {
								margin-top: 30px;
								margin-left: 30px;
							}

							.third-lists {
								margin-left: 60px;
							}
						}
					}
				}
			}

			.copy {
				text-align: center;
				margin-top: 40px;
				padding-bottom: 40px;
				color: rgb(133, 133, 133);
				font-size: 0.8rem;
			}

			.up-to-page {
				position: absolute;
				right: -73px;
				bottom: 25px;
				font-size: 2.8rem;
				color: $background-button;
			}
		}
</style>
