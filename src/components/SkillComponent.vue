<template>
	<div class="skill-container">
		<h2>My Skills</h2>
		<div class="images">
			<div class="image">
				<img src="./img/htcsjs.png">
			</div>
		</div>
		<div class="images">
			<div class="image">
				<img src="./img/bootstrap.png">
			</div>
		</div>
		<div class="images">
			<div class="image flex">
				<img src="./img/Logo-Vuejs.png">
				<img src="./img/ele.png">
			</div>
		</div>
	</div>
</template>
<script>
	export default{
		name : 'SkillComponent'
	}
</script>
<style scoped>
	.skill-container{
		margin-top: 50px;
		width: 100%;
		height: auto;
		text-align: center;
	}
	.skill-container h2{
		font-size: 60px;
		color: #3e3e3e;
		padding: 20px;
	}
	.skill-container .images{
		width: 100%;
		height: auto;
		display: flex;
		align-items: center;
		justify-content: center;
		padding: 20px;
	}
	.skill-container .images .image{
		width: auto;
		height: auto;
	}
	.skill-container .images .image img{
		width: 100%;
		height: 100%;
		max-height: 300px;
		display: inline-block;
	}
	.skill-container .images .image.flex{
		width: 100%;
		padding: 20px;
		display: flex;
		gap: 12px;
		height: auto;
	}
	.skill-container .images .image.flex img{
		width: 50%;
		height: 100%;
		max-height: 300px;
		display: inline-block;
	}
	@media(max-width : 500px){
		.skill-container .images .image.flex img{
			gap: 0;
			margin: 0 5px;
		}
	}
</style>