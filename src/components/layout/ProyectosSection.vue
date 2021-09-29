<template>
	<section id="proyectos">
		<h2>Mis Proyectos</h2>
	</section>
	<div class="p-items">
		<project-base 
		v-for="proyecto in proyectos" 
		:key="proyecto.titulo" 
		:project-titulo="proyecto.titulo"
		:project-image="proyecto.imagen"
		:project-description="proyecto.descripcion"></project-base>
	</div>
</template>

<script>
import projectBase from '../UI/ProjectBase.vue';
import p1 from '../UI/images/p1.png';
import p3 from '../UI/images/p3.png';
import p2 from '../UI/images/p2.jpeg';
import p4 from '../UI/images/p4.png'

export default {
	components: {
		projectBase
	},
	data(){
		return {
			proyectos:[
			{
				titulo:'Sistema CRUD',
				imagen: p1,
				descripcion: 'Sistema CRUD echo con Javascript, AJAX, PHP y Bootstrap'
			},
			{
				titulo:'Aplicación del clima',
				imagen: p2,
				descripcion: 'Una pagina web con el pronostico de mañana de los algunos de los paises de latinoamérica, usa APIREST'
			},
			{
				titulo:'Vibes, red social (en progreso)',
				imagen: p4,
				descripcion: 'Una red social simple usando Vue.js, node.js y firebase'
			},
			{
				titulo:'Monster Slayer',
				imagen: p3,
				descripcion: 'Un minijuego echo principalmente con Javascript usando el framework Vue.js'
			}
			]
		}
	}
}
</script>

<style scoped>
.p-items {
	display: flex;
	flex-direction: row;
	flex-wrap: wrap;
	background-color: rgb(30, 30, 30);
	justify-content: space-around;
}

@media (max-width: 991.98px) {
	.p-items {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
}

section {
	background-color: rgb(50, 120, 150);
	color: white;
}

h2 {
	text-align: center;
	padding: 1em;
}
</style>