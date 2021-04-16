<template>
	<div>
		<h1>Calculator</h1>
		<Calculator />
	</div>
</template>

<script>
	import Calculator from './main/Calculator.vue'

	export default {
		name: 'App',
		components: {
			Calculator
		}
	}
</script>

<style>
	@font-face {
		font-family: 'RobotoMono';
		src: url('./fonts/RobotoMono-Thin.ttf');
	}

	* {
		font-family: 'RobotoMono', sans-serif;
		box-sizing: border-box;
	}

	html, body {
		margin: 0;
		padding: 0;
	}

	#app {
		height: 100vh;

		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		text-align: center;

		color: #fff;
		background: linear-gradient(to right, rgb(83, 105, 118), rgb(41, 46, 73));
	}
</style>
