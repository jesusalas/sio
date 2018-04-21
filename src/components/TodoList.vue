<template>
   <div>
      <h1>Lista de tareas</h1>
      <ul class= "list-group">
         <TodoItem v-for="todo in todos" :item="todo" :key="todo"/>
      </ul>
   </div>
</template>

<script>
import TodoItem from '@/components/TodoItem';
   export default{
      props: ['todos'],
      name: 'TodoList',
      components: {
         TodoItem,
      },
      
   };
</script>

<style>
   .TodoList{
      color: #333;
   }
   
</style>