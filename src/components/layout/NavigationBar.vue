<template>
	<div class="select-menu">
		<span @click="displayMenu">Menu</span>
	</div>
	<transition>
		<nav v-if="menuButton">
			<ul>
				<a href="#header"><li>Acerca de mi</li></a>
				<a href="#proyectos"><li>Mis proyectos</li></a>
				<a href="#conocimientos"><li>Mis conocimientos</li></a>
				<a href="#contacto"><li>Contactame</li></a>
			</ul>
		</nav>
	</transition>
</template>

<script>
export default {
	data(){
		return{
			menuButton: false,
		}
	},
	methods:{
		displayMenu(){
			this.menuButton = !this.menuButton;
		}
	}
}
</script>

<style scoped>
span {
	margin-left: 1em;
}

a {
	color: white;
	text-decoration: none;
}

nav {
	background-color: rgba(30, 30, 30, 0.9);
	color: white;
	height: 100%;
	position: fixed;
	width: 60%;
	margin-top: 54px;
}

ul {
	list-style: none;
}

ul li {
	padding: 1em;
}

ul li:hover {
	background-color: rgb(50, 120, 150);
	cursor: pointer;
}

.select-menu {
	background-color: #333399;
	color: white;
	font-weight: 800;
	position: absolute;
	width: 100%;
	padding: 1em 0em 1em 0em;
}

.select-menu:hover {
	cursor: pointer;
}

.v-enter-from,.v-leave-to {
	transform: translateX(-200px);
	opacity: 0;
}

.v-enter-active,.v-leave-active {
	transition: 0.3s;
}

.v-enter-to,.v-leave-from {
	transform: translateX(0px);
	opacity: 1;
}
</style>