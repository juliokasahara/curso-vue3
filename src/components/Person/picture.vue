<template>
	<img :src="imagem" :alt="descricao"/>
</template>

<script>
export default{
	name: 'Picture',
	data(){
		return{
			imagem:"/img/Vue.png",
			descricao: "vuuuuuuuuuuuuuuuuuuuuuuue!!!!!!!!!!"
		}
	}
}
</script>

