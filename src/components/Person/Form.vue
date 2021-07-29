<template>

	<form action=" " @submit="enviar($event)">
		<label>Curso</label>
		<div>
		<InputText/>
		</div>
		<div>
		<Submit/>
		</div>
	</form>
</template>

<script>
	import InputText from '../Form/InputText.vue'
	import Submit from '../Form/Submit.vue'

	export default {
		name: 'Form',
		components: {
			InputText,
			Submit
		},
	methods: {
		enviar(e){
			e.preventDefault();
			alert('enviado')
		}
	}
	}
</script>
