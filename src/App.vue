<template>

	<div>
		<div>
			<Header />
		</div>
		<h1>Ola App Main</h1>
		<hr>
		<h1>Componente</h1>
		<PrimeiroComponente/>
		<hr>
		<h1>Componente LifeCycle</h1>
		<LifeCycle/>
		<hr>
		<h1>Componente Cadastro</h1>
		<Person/>
	</div>
</template>

<script>
	import Header from './components/home/Header'
	import PrimeiroComponente from './components/PrimeiroComponente.vue'
	import LifeCycle from './components/LifeCycle.vue'
	import Person from './components/Person/Person.vue'

	export default {
		name: 'App',
		components: {
			PrimeiroComponente,
			LifeCycle,
			Person,
			Header
		}
	}
</script>

<style>
		body {
			background-color: #333;
			color: #FFF;
		}

		a {
			color: green;
		}
</style>
