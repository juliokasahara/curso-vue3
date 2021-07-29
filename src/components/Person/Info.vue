<template>
	<div>
		<p v-if="esta_trabalhando"> v-if Trabalhando</p>
		<p v-else> v-else não está Trabalhando</p>
		<ul>
			<li v-for="(tecnoligia, index) in tecnoligias" :key="index"> index = {{index}} - {{tecnoligia}}</li>
		</ul>

		<div>
			<button @click="showEmail">{{ botao }}</button>
		</div>
		<p v-show="mostrar_mail"> {{ email }}</p>
		<p>Portfolio <a :href="meu_link" target="_blank">aqui</a></p>
		<Picture/>

	</div>
</template>

<script>
	import Picture from './picture'

	export default {
		name: 'Info',
		components: {
			Picture,
		},
		data(){
			return{
				esta_trabalhando: false,
				mostrar_mail: true,
				email: 'kkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkkk',
				meu_link: 'http://www.google.com.br',
				botao: 'Mostra',
				tecnoligias: ['Java','Kotlin','Python','PHP','Node']
			}
		},
		methods: {
			showEmail() {
				this.mostrar_mail = !this.mostrar_mail
				if(!this.mostrar_mail){
					this.botao = "Mostra"
				}else{
					this.botao = "Esconde"
				}
			}

		}
	}
</script>
