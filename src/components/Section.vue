<template>
	<div class="container">
	
		<ul>
			<li>{{ suma(2, 2) }}</li>
			<li>{{ saludar("Hello") }}</li>
			<li>Si quieres volar pulsa mas abajo</li>
			<li><button @click="show()">Clickme for show or hide!</button></li>
			<li v-if="isRender">Si vas a volar</li>
			<li v-else>Si no </li>
			<li v-show="isRender">
				If the condition is true, will display this with V_SHOW
			</li>
		</ul>
	</div>
</template>
<script setup>
import { ref } from "vue";
const suma = (a, b) => {
	return `la suma de ${a}+${b}=${a + b}`;
};
const saludar = (name) => `Hello ${name}, wellcome home!`;
let isRender = ref(false);
const show = () => {
	isRender.value = !isRender.value;
};
</script>
<style scoped>
.container {
	display: flex;
	justify-content: center;
	flex-direction: column;
	align-items: center;
	background-color:red;
}
ul {
	display: flex;
	flex-direction: column;
	background-color:red;
}
</style>
