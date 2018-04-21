<template>
   <div>
      <input type="text" @keyup.enter="submit" v-model="todo">
      <button @click="submit">Agregar</button>
   </div>
</template>
<script>
   export default{
      name: 'TodoCreate',
      data(){
         return{
            todo: ''
         }
      },
      methods: {
         submit(){
            
            if (this.todo.length>0) {

               this.$emit('addTodo',{
                  name: this.todo
               });
               this.todo = "";
               
            }
         }
      }
   };
</script>
<style>
</style>