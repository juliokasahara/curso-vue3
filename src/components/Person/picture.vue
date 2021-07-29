<template>
	<div>
	<img :src="imagem" :alt="descricao"/>
	<MudarImagem @mudar-imagem="trocarImagem"/>
	</div>
</template>

<script>
import MudarImagem from './MudarImagem.vue'
export default{
	name: 'Picture',
	components: {
		MudarImagem
	},
	data(){
		return{
			imagem:"/img/Vue.png",
			descricao: "vuuuuuuuuuuuuuuuuuuuuuuue!!!!!!!!!!"
		}
	},
	methods:{
		trocarImagem(){
			this.imagem = "/img/emit.png"
		}
	}
}
</script>

