<template>
	<div class="about-container">
		<h1>About Me</h1>
		<div class="about-flex">
			<h3>HI! I'm Mark Ronald, a junior web developer who enjoys creating websites and coding is my hobby. JavaScript and vue.js are my areas of expertise. I work hard and passionately at what I do.</h3>
		</div>
	</div>
</template>
<script>
	export default{
		name : 'AboutComponent'
	}
</script>
<style scoped>
	.about-container{
		width: 100%;
		height: auto;
		padding: 20px;
		text-align: center;
		background: linear-gradient(247deg, #251426 12%, #3f6290 85%);
		color: aliceblue;
	}
	.about-container h1{
		font-size: 100px;
		display: flex;
		align-items: center;
		justify-content: center;
		color: aliceblue;
	}
	.about-container h1 svg{
		margin-right: 20px;
	}
	.about-container .about-flex{
		width: 100%;
		height: auto;
		padding: 20px;
		display: flex;
		align-items: center;
		justify-content: center;
		gap: 20px;
	}
	.about-container .about-flex h3{
		font-size: 30px;
		font-weight: 500;
		font-family: Courier;
	}
	@media(max-width : 900px){
		.about-container h1{
			font-size: 70px;
		}
		.about-container .about-flex h3{
			font-size: 22px;
		}
	}
</style>