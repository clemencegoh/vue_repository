<template>
	<div class="todoListWrapper">
		<TodoComponent/>
	</div>
</template>

<script>
	import TodoComponent from "@/components/TodoComponent";

	export default {
		name: "TodoList",
		components: {
			TodoComponent
		},
	}
</script>