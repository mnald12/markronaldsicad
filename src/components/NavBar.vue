<template>
	<nav class="desktop" v-if="isDesktop" :style="{background : bgd}">
		<div class="brand-name">
			<h3 :style="{color : clr}">
				Mark Ronald
			</h3>
		</div>
		<div class="links">
			<button :style="{color : clr}" class="link-btn"><svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-github" viewBox="0 0 16 16"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg></button>
			<button :style="{color : clr}" class="link-btn"><svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-linkedin" viewBox="0 0 16 16"><path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z"/></svg></button>
			<button :style="{color : clr}" class="link-btn"><svg xmlns="http://www.w3.org/2000/svg" width="30" height="30" fill="currentColor" class="bi bi-facebook" viewBox="0 0 16 16"><path d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951z"/></svg></button>
			<button :style="{color : clr, borderColor : clr}" class="link-big-btn">Hire me</button>
		</div>
	</nav>
	<nav class="desktop" v-else-if="isPhone" :style="{background : bgd}">
		<div class="brand-name">
			<h3 :style="{color : clr}">
				Mark Ronald
			</h3>
		</div>
		<div class="links">
			<button :style="{color : clr}" class="link-btn"><svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor" class="bi bi-github" viewBox="0 0 16 16"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg></button>
			<button :style="{color : clr}" class="link-btn"><svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor" class="bi bi-linkedin" viewBox="0 0 16 16"><path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z"/></svg></button>
			<button :style="{color : clr}" class="link-btn"><svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor" class="bi bi-facebook" viewBox="0 0 16 16"><path d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951z"/></svg></button>
			<button :style="{color : clr, borderColor : clr}" class="link-big-btn">Hire me</button>
		</div>
	</nav>
</template>
<script>
	export default{
		name : 'NavBar',
		data(){
			return{
				isDesktop : true,
				isPhone : false,
				bgd : 'transparent',
				scrl : window.scrollY,
				clr : 'aliceblue'
			}
		},
		mounted(){
			window.addEventListener("resize", this.reSize)
			window.addEventListener('scroll', this.scrolls)
		},
		unmounted(){
			window.removeEventListener("resize", this.reSize)
			window.addEventListener('scroll', this.scrolls)
		},
		methods : {
			reSize(){
				this.width = window.innerWidth
				this.height = window.innerHeight
				if(this.width >= 900){
					this.isDesktop = true
					this.isPhone = false
				}
				else{
					this.isPhone = true
					this.isDesktop = false
				}
			},
			scrolls(){
				if(this.scrl < window.scrollY){
					this.isDesktop = false
					this.isPhone = false
					this.scrl = window.scrollY
				}
				else{
					if(window.innerWidth >= 900) this.isDesktop = true
					else this.isPhone = true
					this.scrl = window.scrollY
				}
				if(this.scrl >= 250){
					this.clr = 'black'
					this.bgd = 'rgba(255, 255, 255, 0.50)'
				}
				else{
					this.clr = 'aliceblue'
					this.bgd = 'transparent'
				}
			}
		},
		beforeMount(){
			let width = window.innerWidth
			if(width >= 900){
				this.isDesktop = true
				this.isPhone = false
			}
			else{
				this.isDesktop = false
				this.isPhone = true
			}
			if(window.scrollY == 0){
				this.isPhone = false
				this.isDesktop = false
			}
		}
	}
</script>
<style scoped>
	.desktop{
		width: 100%;
		height: 70px;
		display: flex;
		align-items: center;
		position: fixed;
		top: 0;
		transition: 0.50s;
		animation: goDown 1s ease-in-out;
		z-index: 999;
	}
	.desktop .brand-name{
		width: auto;
		height: auto;
		position: absolute;
		left: 20px;
		text-align: left;
	}
	.desktop .brand-name h3{
		color: aliceblue;
		font-weight: 400;
		font-size: 20px;
	}
	.desktop .brand-name h3:hover{
		transform: scale(1.2);
	}
	.desktop .links{
		width: auto;
		height: auto;
		display: flex;
		align-items: center;
		position: absolute;
		right: 20px;
	}
	.desktop .links .link-btn{
		outline: none;
		border: none;
		padding: 0 12px;
		background: transparent;
		color: aliceblue;
		font-size: 17px;
		cursor: pointer;
		transition: 0.40s;
	}
	.desktop .links .link-btn:hover{
		transform: scale(1.1);
	}
	.desktop .links .link-big-btn{
		outline: none;
		border: none;
		padding: 8px 12px;
		background: transparent;
		color: aliceblue;
		font-size: 17px;
		cursor: pointer;
		border: 1px solid aliceblue;
		border-radius: 3px;
		margin-left: 6px;
	}
	.phone{
		width: 100%;
		height: 70px;
		display: flex;
		align-items: center;
		position: fixed;
		top: 0;
		transition: 0.50s;
		animation: goDown 1s ease-in-out;
		z-index: 999;
	}
	.phone .brand-name{
		width: auto;
		height: auto;
		position: absolute;
		left: 20px;
		text-align: left;
	}
	.phone .brand-name h3{
		color: aliceblue;
		font-weight: 400;
		font-size: 20px;
	}
	.phone .links{
		width: auto;
		height: auto;
		display: flex;
		align-items: center;
		position: absolute;
		right: 20px;
	}
	.phone .links .link-btn-menu{
		outline: none;
		border: none;
		padding: 5px;
		background: transparent;
		color: aliceblue;
		font-size: 17px;
		cursor: pointer;
		transition: 0.40s;
	}
	@keyframes goDown{
		from{
			transform: translateY(-100%);
		}
		to{
			transform: translateY(0);
		}
	}
</style>