<script>
export default {
	name: "NavComponent",
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
  
    <ul>
        <li>
            <a href="#">
                Home 
                <i class="fa-solid fa-angle-down"></i>

                <div class="dropdown-content">

                    <ul>
                        <li><strong>Overview</strong></li>
                        <li>Get inspired</li>
                        <li>What customer say</li>
                        <li>About us</li>
                        <li>Contact us</li>
                    </ul>  

                </div>
                
            </a>
        </li>
        <li>
            <a href="#">
                Pages <i class="fa-solid fa-angle-down"></i>
            </a>
        </li>
        <li>
            <a href="#">
                Courses <i class="fa-solid fa-angle-down"></i>
            </a>
        </li>
        <li>
            <a href="#">
                Features <i class="fa-solid fa-angle-down"></i>
            </a>
        </li>
        <li>
            <a href="#">
                Blog <i class="fa-solid fa-angle-down"></i>
            </a>
        </li>
        <li>
            <a href="#">
                Shop <i class="fa-solid fa-angle-down"></i>
            </a>
        </li>
    </ul>

</template>

<style lang="scss" scoped>
    @use "../assets/scss/partials/variables.scss" as *;
	ul {
		display: flex;
		list-style-type: none;

		li {
			
			a {
				text-decoration: none;
				color: black;
				padding-right: 30px;
				font-size: 1rem;
                color: $font-color-secondary;

				& i {
					font-size: xx-small;
				}
			}
		}
	}
</style>
