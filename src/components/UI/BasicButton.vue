<template>
	<a :href="anchorTag" target="_blank" rel="noopener noreferrer">
	<button>
		<slot></slot>
	</button>
	</a>
</template>

<script>
export default {
	props: ['anchorTag']
}
</script>

<style scoped>
button {
	padding: 1em;
	border: 0px;
	color: white;
	background-color: rgb(30, 30, 30);
	border: 1px solid rgb(50, 120, 150);
	border-radius: 5px;
	margin: 0em 6em 3.50em 6em;
	transition: 0.1s;
}

button:hover {
	cursor: pointer;
	background-color: rgb(50, 120, 150);
	box-shadow: 0px 0px 10px rgb(50, 180, 300);
}
</style>