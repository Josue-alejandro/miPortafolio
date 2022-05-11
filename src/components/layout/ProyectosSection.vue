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
		:project-description="proyecto.descripcion"
		:project-link="proyecto.link"></project-base>
	</div>
</template>

<script>
import projectBase from '../UI/ProjectBase.vue';
import p1 from '../UI/images/p1.png';
import p3 from '../UI/images/p3.png';
import p2 from '../UI/images/p2.png';
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
				descripcion: 'Sistema CRUD hecho con Javascript, AJAX, PHP y Bootstrap.',
				link: 'https://github.com/Josue-alejandro'
			},
			{
				titulo:'Aplicación del clima',
				imagen: p2,
				descripcion: 'Web que muestra el clima de las ciudades del mundo, hecha con Vue.js y API rest.',
				link: 'https://weatherappjosh.netlify.app/'
			},
			{
				titulo:'Gajelici, e-commerce',
				imagen: p4,
				descripcion: 'Tienda online hecha con Wordpress',
				link: 'https://gajelici.com/'
			},
			{
				titulo:'Monster Slayer',
				imagen: p3,
				descripcion: 'Un minijuego hecho principalmente con Javascript usando el framework Vue.js',
				link: 'https://github.com/Josue-alejandro'
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
	padding-top: 5em;
	padding-bottom: 5em;
}

@media (max-width: 991.98px) {
	.p-items {
		display: flex;
		flex-direction: column;
		align-items: center;
	}
}

section {
	background-color: #333399;
	color: white;
}

h2 {
	text-align: center;
	padding: 1em;
}
</style>