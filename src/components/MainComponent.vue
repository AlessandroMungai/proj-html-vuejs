<script>
import JumboComponent from '../components/sections/JumboComponent.vue';
import SecondSection from '../components/sections/SecondSection.vue';
import ThirdSection from '../components/sections/ThirdSection.vue';
import FourthSection from '../components/sections/FourthSection.vue';
import FifthSection from '../components/sections/FifthSection.vue';
import SixthSection from '../components/sections/SixthSection.vue';
import SeventhSection from '../components/sections/SeventhSection.vue';
import EighthSection from '../components/sections/EighthSection.vue';

export default {
	name: "MainComponent",
	components: {
		JumboComponent,
		SecondSection,
		ThirdSection,
		FourthSection,
		FifthSection,
		SixthSection,
		SeventhSection,
		EighthSection
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

		<div class="fifth-section">

			<FifthSection />

		</div>

		<div class="sixth-section">

			<SixthSection />

		</div>

		<div class="seventh-section">

			<SeventhSection />

		</div>

		<div class="eighth-section">

			<EighthSection />

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
	.fifth-section {
		margin-top: 100px;
	}
	.sixth-section {
		margin-top: 150px;
	}
	.seventh-section {
		margin-top: 75px;
	}
	.eighth-section {
		margin-top: 50px;
	}
</style>
