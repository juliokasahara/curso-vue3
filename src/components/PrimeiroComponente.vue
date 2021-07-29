<template>
	<div>
		<h3>Ola Vue Componente</h3>
		<p>{{ nome }} - {{profisao}}</p>
	</div>
</template>

<script>
export default {
	name: 'PrimeiroComponente',
	data() {
		return {
			nome:"Julio",
			profisao:"Dev"
		}
	},
}
</script>
