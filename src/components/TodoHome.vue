<template>
	<div>
		<TodoCreate @addTodo="addTodo"/>
		<TodoList v-bind:todos="todos"/>
	</div>
</template>

<script>
import TodoList from '@/components/TodoList';
import TodoCreate from '@/components/TodoCreate';
import axios from 'axios';

export default{
	name:'Home',
		components:{
			TodoList,
			TodoCreate
	},
	data() {
		return {
			todos:[]
		};
	},

	mounted(){
		//TODO: obetener datos mediante un api
		this.fetchTodo();
	},
	methods:{
		fetchTodo(){
			axios.get('http://172.16.1.39:5000/api/todo')
			.then(({ data }) =>{
				this.todos = data.todos;
			});
		},
		addTodo(newTodo){
			var exists = false;
			
			this.todos.forEach(function(element){
				if (element.name == newTodo.name){
            		exists =true
            	}
         	});

	        if (!exists) {this.todos.push(newTodo);}
	        
		}
	},
};
</script>

<style scoped>
	.Home{
		color: red;
	}
	
</style>