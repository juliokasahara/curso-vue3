<template>
	<h3>Meu nome é: {{ nome }}</h3>
</template>

<script>
export default {
	name: 'LifeCycle',
	data() {
		return {
			nome: 'Ainda não sei!!'
		}
	},

	created() {
		setTimeout(() => {
			this.nome = 'Criaçao (created)'
		},1000)
	},
	mounted() {
		setTimeout(() => {
			this.nome = 'Montado (mounted)'
		},2000);
			this.lifeCycle();
	},
	methods: {
		lifeCycle(){
			console.log("executado!!!!!!!")
		}
	}
}
</script>
