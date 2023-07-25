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
            <a class="title-menu" href="#">
                Home 
                <i class="fa-solid fa-angle-down"></i>
            </a>

            <div class="dropdown-content">
                <ul>
                    <li><a href="#">Start Here</a></li>
                    <li><a href="#">Success Story</a></li>
                    <li><a href="#">About Me</a></li>
                    <li><a href="#">About us 01</a></li>
                    <li><a href="#">About us 02</a></li>
                    <li><a href="#">About us 03</a></li>
                    <li><a href="#">Contact Me</a></li>
                    <li><a href="#">Contact Us</a></li>
                    <li><a href="#">Purchase Guide</a></li>
                    <li><a href="#">Privacy Policy</a></li>
                    <li><a href="#">Terms Of Service</a></li>
                </ul>  
            </div>
        </li>

        <li>
            <a class="title-menu" href="#">
                Pages <i class="fa-solid fa-angle-down"></i>
            </a>
            <div class="dropdown-content">
                <ul>
                    <li><a href="#">Start Here</a></li>
                    <li><a href="#">Success Story</a></li>
                    <li><a href="#">About Me</a></li>
                    <li><a href="#">About us 01</a></li>
                    <li><a href="#">About us 02</a></li>
                    <li><a href="#">About us 03</a></li>
                    <li><a href="#">Contact Me</a></li>
                    <li><a href="#">Contact Us</a></li>
                    <li><a href="#">Purchase Guide</a></li>
                    <li><a href="#">Privacy Policy</a></li>
                    <li><a href="#">Terms Of Service</a></li>
                </ul>  
            </div>
        </li>

        <li>
            <a class="title-menu" href="#">
                Courses <i class="fa-solid fa-angle-down"></i>
            </a>
            <div class="dropdown-content">
                <ul>
                    <li><a href="#">Start Here</a></li>
                    <li><a href="#">Success Story</a></li>
                    <li><a href="#">About Me</a></li>
                    <li><a href="#">About us 01</a></li>
                    <li><a href="#">About us 02</a></li>
                    <li><a href="#">About us 03</a></li>
                    <li><a href="#">Contact Me</a></li>
                    <li><a href="#">Contact Us</a></li>
                    <li><a href="#">Purchase Guide</a></li>
                    <li><a href="#">Privacy Policy</a></li>
                    <li><a href="#">Terms Of Service</a></li>
                </ul>  
            </div>
        </li>
        
        <li>
            <a class="title-menu" href="#">
                Features <i class="fa-solid fa-angle-down"></i>
            </a>
        </li>
        <li>
            <a class="title-menu" href="#">
                Blog <i class="fa-solid fa-angle-down"></i>
            </a>
        </li>
        <li>
            <a class="title-menu" href="#">
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
		position: relative;	
            .dropdown-content {
                width: 180px;
                display: none;
                position: absolute;
                top: 30px;
                background-color: whitesmoke;
                padding-left: 16px;
                padding-top: 20px;
                padding-bottom: 20px;
                border-bottom: 3px solid $background-button;

                ul {
                    display: flex;
                    flex-direction: column;

                    li{
                        margin-bottom: 20px;
                    }
                }
            }

            &:hover .title-menu {
                color: $background-button;
                text-decoration: underline;
            }
            &:hover .dropdown-content {
                display: block;
            }

			a {
				text-decoration: none;
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
