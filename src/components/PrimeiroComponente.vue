<template>
	<div>
		<h3>Ola Vue Componente</h3>
		<p>{{ nome }} - {{profisao}}</p>
		<MultEvent />

		<hr>
			<Reutilizacao />
		<hr>
			<Reutilizacao />
		<hr>
			<Reutilizacao />
		<hr>
	</div>
</template>

<script>
import MultEvent from "./MultEvent.vue"
import Reutilizacao from "./Form/Reutilizacao"

export default {
	name: 'PrimeiroComponente',
	components: {
		MultEvent,
		Reutilizacao
	},
	data() {
		return {
			nome:"Julio",
			profisao:"Dev"
		}
	},
}
</script>
