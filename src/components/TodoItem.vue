<template>
<li class= "list-group-item">
	{{item.name}}
</li>
</template>

<script>
	export default{
		props: ['item'],
		name: 'TodoItem',
	};
</script>

<style>
	.TodoList{
		color: #333;
	}
	
</style>