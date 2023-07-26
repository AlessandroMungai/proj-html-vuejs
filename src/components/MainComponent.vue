<script>
import JumboComponent from '../components/sections/JumboComponent.vue';
import SecondSection from '../components/sections/SecondSection.vue';
import ThirdSection from '../components/sections/ThirdSection.vue';
import FourthSection from '../components/sections/FourthSection.vue';

export default {
	name: "MainComponent",
	components: {
		JumboComponent,
		SecondSection,
		ThirdSection,
		FourthSection
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

			<JumboComponent />

		</div>
		
		<div class="second-section">

			<SecondSection />
			
		</div>

		<div class="third-section">

			<ThirdSection />

		</div>

		<div class="fourth-section">

			<FourthSection />

		</div>

    </main>

</template>

<style lang="scss" scoped>
	@use "../assets/scss/partials/variables.scss" as *;
	.second-section {
		padding-top: 140px;
	}
	.third-section {
		padding-top: 100px;
		
	}
	.fourth-section {
		padding-top: 100px;
		
	}
</style>
