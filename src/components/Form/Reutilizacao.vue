<template>
	<div>
		<button @click="ativar">Clique aqui</button>
		<span v-show="flg">Ativado!</span>
	</div>
</template>

<script>

export default {
	name: "Reutilizacao",
	data() {
		return {
			flg: false
		}
	},
	methods: {
		ativar(){
			this.flg = !this.flg
		}
	},
}
</script>
