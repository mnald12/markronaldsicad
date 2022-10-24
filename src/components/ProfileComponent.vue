<template>
	<div class="profile-container">
		<div class="image">
			<img src="./img/self.png">
		</div>
		<div class="info">
			<h1>HELLO</h1>
			<p>I'm</p>
			<h2>Mark Ronald Sicad</h2>
			<h3>Junior Web Developer</h3>
		</div>
	</div>
</template>
<script>
	export default{
		name : 'ProfileComponent'
	}
</script>
<style scoped>
	.profile-container{
		width: 100%;
		height: auto;
		min-height: 560px;
		display: flex;
		align-items: center;
		justify-content: center;
		background: linear-gradient(to bottom right, #5b05dc 0%, #218291 98%);
		background-size: 100% 50%;
		background-repeat: no-repeat;
		gap: 40px;
		animation: backDown 1s ease-in-out;
	}
	@keyframes backDown{
		from{
			background-size: 100% 0;
		}
		to{
			background-size: 100% 50%;
		}
	}
	.profile-container .image{
		width: 280px;
		height: 280px;
		border-radius: 50%;
		overflow: hidden;
		background: linear-gradient(to left, royalblue, aliceblue);
		animation: rot1 ease-in-out 20s alternate infinite;
		z-index: 1;
	}
	.profile-container .info{
		width: auto;
		min-width: 50%;
		height: auto;
		overflow: hidden;
		padding: 12px;
		text-align: left;
	}
	.profile-container .info h1{
		font-size: 100px;
		color: aliceblue;
		padding: 20px 0;
	}
	.profile-container .info p{
		font-size: 20px;
		color: #0a0a0a;
		display: inline-block;
	}
	.profile-container .info h2{
		font-size: 60px;
		color: #3e3e3e;
	}
	.profile-container .info h3{
		font-size: 30px;
		color: aliceblue;
		padding: 12px;
		border-radius: 2px;
		background: linear-gradient(royalblue, darkblue);
		display: inline-block;
	}
	.profile-container .image img{
		width: 100%;
		height: 100%;
		animation: rot2 ease-in-out 20s alternate infinite;
	}
	@keyframes rot1{
		from{
			transform: rotate(360deg);
		}
		to{
			transform: rotate(0);
		}
	}
	@keyframes rot2{
		from{
			transform: rotate(0);
		}
		to{
			transform: rotate(360deg);
		}
	}
	@media (max-width : 900px){
		.profile-container{
			flex-wrap: wrap;
		}
		.profile-container .image{
			margin-top: 60px;
			width: 250px;
			height: 250px;
		}
		.profile-container .info{
			text-align: center;
		}
		.profile-container .info h1{
			padding: 12px;
			color: #3e3e3e;
			font-size: 80px;
		}
		.profile-container .info h2{
			color: #3e3e3e;
			font-size: 40px;
		}
		.profile-container .info h3{
			font-size: 30px;
		}
	}
</style>