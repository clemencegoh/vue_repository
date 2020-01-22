<template>
	<div>
		<span>Hello World from todo Component!</span>
		<br>
		<span>Current Count: {{ count }}</span>
		<br>
		<br>
		<button v-on:click="increaseCount()"> Click here to increment count </button>
	</div>
</template>

<script>
	export default {
		name: "TodoComponent",
		computed: {
			count() {
				return this.$store.state.count;
			},
		},
		methods: {
			increaseCount(){
				return this.$store.commit({
					type: 'increaseCount',
					amount: 2,
				});
			}
		}
	}
</script>

<style scoped>
	span{
		color: darkred;
	}
</style>