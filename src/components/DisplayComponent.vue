<template>
	<div class="display-container">
		<div class="display-welcome" id="welcome">
			<div v-for="(ball, i) in balls" :style="{width : ball.width, height : ball.height, left : ball.left, top : ball.top, background : ball.bgd}" :key="i" class="ball"></div>
			<h1>W E L C O M E</h1>
			<h3>TO MY</h3>
			<h1>PORTFOLIO</h1>
		</div>
	</div>
</template>
<script>
	export default{
		name : 'DisplayComponent',
		data(){
			return {
				balls : [],
				colors : ['linear-gradient(70deg, #2ec297 28%, #c6cffe 76%)', 'radial-gradient(ellipse farthest-corner at bottom right, #890eee 34%, #acd65f 97%)', 'linear-gradient(to left, #0e31f7 11%, #2e8deb 66%)', 'radial-gradient(circle farthest-side at left, #9a9cf9 27%, #1163a7 73%)', 'linear-gradient(234deg, #ef6625 19%, #b3c174 92%)', 'linear-gradient(115deg, #a940a9 3%, #83d519 67%)', 'linear-gradient(to top, rgb(157, 57, 206) 38%, rgb(193, 179, 226) 56%)', 'linear-gradient(to top, #9c72cb 19%, #fa5c6d 87%)'],
				rand : function(n){
					return Math.floor(Math.random() * n)
				}
			}
		},
		methods : {
			changePos(){
				for(let i of this.balls){
					let s = this.rand(200) + 20 + 'px'
					i.width = s
					i.height = s
					i.left = this.rand(1000) + 'px'
					i.top = this.rand(320) + 'px'
					i.bgd = this.colors[this.rand(this.colors.length)]
				}
			}
		},
		beforeMount(){
			for(let i = 0; i < 10; i++){
				let s = this.rand(200) + 20 + 'px'
				let b = {
					width : s,
					height : s,
					left : this.rand(1000) + 'px',
					top : this.rand(320) + 'px',
					bgd : this.colors[this.rand(this.colors.length)]
				}
				this.balls.push(b)
			}
		},
		mounted(){
			setInterval(this.changePos, 5000)
		}
	}
</script>
<style scoped>
	.display-container{
		width: 100%;
		height: auto;
		padding: 20px;
		min-height: 400px;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.display-container .display-welcome{
		width: 100%;
		height: auto;
		padding: 50px 0;
		position: relative;
		overflow: hidden;
	}
	.display-container .display-welcome h3{
		font-size: 40px;
		padding: 20px;
		color: white;
		text-shadow: -2px 3px 5px #1e1e1e;
	}
	.display-container .display-welcome h1{
		font-size: 100px;
		padding: 20px;
		text-shadow: -2px 3px 5px #1e1e1e;
		color: white;
	}
	.display-container .display-welcome .ball{
		position: absolute;
		background: forestgreen;
		border-radius: 50%;
		z-index: -1;
		transition: 2s;
	}
	@media (max-width : 900px){
		.display-container .display-welcome h1{
			font-size: 40px;
			padding: 12px;
		}
		.display-container .display-welcome h3{
			padding: 8px;
			font-size: 20px;
		}
	}
</style>