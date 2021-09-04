<template>
	<header :style="{ height: heightScreen + 'px'}"  id="header">
		<div class="port">
			<h1>Josue Alejandro</h1>
			<p>¡Hola!, Soy desarrollar web tengo 19 años y vivo en Maracaibo una ciudad de Venezuela, principalmente me gusta el front-end, pero tambien puedo hacer back-end, en este portafolio puedes encontrar información sobre mis proyectos y algunos de mis conocimientos.</p>
			<basic-button anchor-tag="#contacto">Contactame</basic-button>
		</div>
	</header>
</template>

<script>
export default {
	setup(){
		const screen = window.screen;
		const heightScreen = screen.height;

		return {heightScreen};
	}
}
</script>

<style scoped>
header {
	text-align: center;
	background: url('./Header.jpg') center center;
	background-size: 220%;
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	color: white;
	background-size: 100%;
}

.port {
	background-color: rgba(0, 0, 0, 0.7);
	height: 100%;
	display: flex;
	flex-direction: column;
	justify-content: center;
	align-items: center;
	padding-left: 400px;
	padding-right: 400px;
}

@media (max-width: 991.98px) {
	.port {
		padding-left: 30px;
		padding-right: 30px;
	}
	header {
		background-size: 250%;
	}
}

.port h1 {
	margin-bottom: 30px;
}

.port p {
	margin-bottom: 2em;
}
</style>