
<template>
	<div id="app">
		<div id="head">
			<p>Регистрация</p>
		</div>
		<router-view/>
	</div>
</template>

<style>
	body {
		width: 100%;
		margin: 0;
		height: 500px;
		/*padding: auto;*/
	}
	#head {
		position: fixed;
		width: 100%;
		height: 56px;
		left: 0px;
		top: 0px;
		background: #C4C4C4;
		text-align: left;
		padding: auto;
	}
	#head p {
		font-weight: 500;
		font-size: 20px;
		margin: 16px 10px;
	}
	#app {
		font-family: 'Roboto', sans-serif;
		/*-webkit-font-smoothing: antialiased;*/
		/*-moz-osx-font-smoothing: grayscale;*/
		text-align: center;
		display: block;
	}
</style>
