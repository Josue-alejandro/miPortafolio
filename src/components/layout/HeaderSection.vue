<template>
	<header :style="{ height: heightScreen + 'px'}"  id="header">
		<div class="port">
			<ul class="title-list">
				<li>
					<h1>😎 Josue Alejandro</h1>
					<h1>👨‍💻 Desarrollador Web</h1>
					<h1>📓 Portafolio Web</h1>
				</li>
			</ul>
			<p>Soy desarrollador web orientado principalmente al front-end y con conocimientos solidos en back-end. Tengo 20 años y desde muy joven me senti interesado por el mundo de la programación. En este portafolio podras encontrar enlaces a los diferentes proyectos que he desarrollado.</p>
			<basic-button anchor-tag="https://drive.google.com/file/d/1F75YEQY5dAFAyS-AcMvqJ_kQPfON_pQV/view?usp=sharing">Descargar CV</basic-button>
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
.title-list {
	list-style: none;
	height: 40px;
	overflow: hidden;
	margin-bottom: 20px;
	line-height: 40px;
}

@keyframes cambiar {
	0%{margin-top: 0px;}
	20%{margin-top: 0px;}

	25%{margin-top: -40px;}
	50%{margin-top: -40px;}

	55%{margin-top: -80px;}
	80%{margin-top: -80px;}

	85%{margin-top: -40px;}
	95%{margin-top: -40px;}

	100%{margin-top: 0px;}
}

.title-list li {
	padding-left: 0px;
	animation: cambiar 7s infinite;
}

.title-list li h1 {
	padding-bottom: 0px;
	margin-bottom: 0px;
}

header {
	text-align: center;
	background: url('./Header.jpg') center center;
	background-position: center center;
	background-repeat: no-repeat;
	background-attachment: fixed;
	background-size: cover;
	background-color: #333399;
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	color: white;
}

.port {
	background-color: rgba(0, 0, 0, 0.3);
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