<template>
	<section id="conocimientos">
		<h2>Mis conocimientos</h2>
	</section>
	<div class="carrusel">
		<div>
			<div class="texto">
				<span class="icon-window" style="font-size: 80px; color: rgb(0,180,300);"></span>
				<h3>Front-end</h3>
				<p>Mi parte favorita del desarrollo web es el front-end y toda la creatividad que se puede expresar en ello, cuento con conocimientos solidos en las siguientes tecnologías</p>
			</div>
			<ul>
				<li>HTML</li>
				<li>CSS</li>
				<li>Javascript</li>
				<li>Vue.js</li>
				<li>React</li>
				<li>Bootstrap, Materialize</li>
			</ul>
		</div>
		<div>
			<div class="texto">
				<span class="icon-database" style="font-size: 80px; color: rgb(300,200,40);"></span>
				<h3>Back-end</h3>
				<p>Tengo buenos conocimientos en códigos de programación del lado del servidor y para programar bases de datos</p>
			</div>
			<ul>
				<li>Node.js</li>
				<li>MongoDB</li>
				<li>PHP</li>
				<li>SQL</li>
			</ul>
		</div>
	</div>
</template>

<style scoped>
@media (max-width: 767.98px) {
	.carrusel {
		display: flex;
		flex-direction: column;
	}

	ul {
		padding-left: 0px;
	}
}

section {
	background-color: #333399;
	color: white;
}

h2 {
	padding: 1em;
	text-align: center;
}

.carrusel {
	background-color: rgb(30, 30, 30);
	color: white;
	text-align: center;
	display: flex;
	flex-direction: row;
	flex-wrap: wrap;
	justify-content: space-around;
	padding-top: 5em;
	padding-bottom: 5em;
}

.carrusel div {
	padding: 1em 0em 1em 0em;
	width: 400px;
}

@media (max-width: 991.98px) {
	.carrusel div{
		width: auto;
	}

	
}

ul {
	list-style: none;
	padding: 1em;
}

.texto {
	padding: 0px;
}

.texto h3 {
	padding: 1em;
}
</style>