<template>
	<div>
		<img :src="projectImage">
		<h2>{{ projectTitulo }}</h2>
		<p>{{ projectDescription }}</p>
		<basic-button anchor-tag="https://github.com/Josue-alejandro">Ver en Github</basic-button>
	</div>
</template>

<script>
export default {
	props: ['projectTitulo', 'projectImage', 'projectDescription']
}
</script>

<style scoped>
div {
	width: 100%;
	max-width: 400px;
	display: flex;
	flex-direction: column;
	text-align: center;
	color: white;
	background-color: rgb(30, 30, 30);
}

div img {
	padding: 1em 2em 0em 2em;
	height: 200px;
}

div h2 {
	margin-top: 2em;
	margin-bottom: 0.50em;
}

div p {
	margin-bottom: 2em;
	height: 40px;
}
</style>