<template>
	<div>
		<h3>Cadastro pessoa: {{ nome }}</h3>
		<Info/>
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
				nome: 'Julio'
			}
		}
	}
</script>
