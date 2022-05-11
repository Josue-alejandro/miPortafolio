<template>
	<div>
		<img :src="projectImage">
		<h3><strong>{{ projectTitulo }}</strong></h3>
		<p>{{ projectDescription }}</p>
		<basic-button :anchor-tag="projectLink">Ver página</basic-button>
	</div>
</template>

<script>
export default {
	props: ['projectTitulo', 'projectImage', 'projectDescription', 'projectLink']
}
</script>

<style scoped>
div {
	width: auto;
	max-width: 300px;
	display: flex;
	flex-direction: column;
	text-align: center;
	color: white;
	background-color: rgb(30, 30, 30);
	-webkit-box-shadow: 0px 0px 15px 5px #000000; 
	box-shadow: 0px 0px 15px 5px #000000;
	border-radius: 10px;
	padding: 1em;
	margin: 1em;
}

div img {
	height: 200px;
	border-radius: 10px;
}

div h3 {
	font-weight: bold;
	padding-bottom: 10px;
	padding-top: 10px;
}

div p {
	height: 40px;
	font-size: 14px;
	margin-bottom: 20px;
}

@media (max-width: 991.98px) {
	div{
		width: 80%;
		margin: 0px;
		margin-bottom: 1em;
	}

	
}
</style>