<template>
	<div>
		<button @click="primeiro(variavel,$event),segundo($event),apaga($event)"> ativar N eventos</button>
		<p>{{ texto }}</p>
	</div>
</template>

<script>

export default ({
	name: 'MultEvent',
	data() {
		return {
			texto: "",
			variavel: "primeiro"
		}
	},
	methods: {
		primeiro(variavel,e){
			this.texto = variavel;
		},
		segundo(e){
			setTimeout(() => this.texto = "segundo", 500)
		},
		apaga(e){
			setTimeout(() => this.texto = "", 1000)
		}
	}
})
</script>
