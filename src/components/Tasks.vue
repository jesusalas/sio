<template>
   <div class="container">
      <h1>Lista de tareas</h1>
      <ul class="list-group">
         <li v-for="task in tasks" class="list-group-item"> {{task.empleado}}</li>
      </ul>
   </div>
</template>
<script>
   import axios from "axios"

   var urlRoute = 'http://172.16.1.107:8000/api/cedis/1/employees'

   export default {
      name: 'Tasks',
      created: function(){
         this.getRoutes();
      },
      data () {
         return {
              tasks: []
         }
      },
      methods:{
         getRoutes: function(){
            axios.get(urlRoute).then(response => {
               this.tasks = response.data.data;
            });
         }
      },
   }

</script>
<style>
    
</style>