<template>
	<div>
		<h3>Ola Vue Componente</h3>
		<p>{{ nome }} - {{profisao}}</p>
		<MultEvent />
	</div>
</template>

<script>
import MultEvent from "./MultEvent.vue"
export default {
	name: 'PrimeiroComponente',
	components: {
		MultEvent
	},
	data() {
		return {
			nome:"Julio",
			profisao:"Dev"
		}
	},
}
</script>
