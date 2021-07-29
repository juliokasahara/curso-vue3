<template>
	<div>
		<h3>Cadastro pessoa: {{ nome }}</h3>
		<Info props="Dado envidado via props Person.vue -> Info.vue" :propsBind="propsBind"/>
		<hr>
		<Form/>
	</div>
</template>

<script>
	import Info from './Info'
	import Form from './Form'

	export default {
		name: 'Person',
		components:{
			Info,
			Form
		},
		data() {
			return {
				nome: 'Julio',
				propsBind: 'Dado enviado por Bind no props'
			}
		}
	}
</script>
