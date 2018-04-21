<template>
   
   <div class="container">
      <div class="row">
         <div class="col-sm-8">
            <ul class="list-group">
               <li class="list-group-nav">
                  <nav class="navbar navbar-dark bg-primary">
                     <form class="form-inline">
                        <a class="navbar-brand" href="#">Empleado</a>
                        <input type="text" placeholder="Buscar" class="form-control" v-model="employee">
                        <div class="btn-group">
                           <select id="inputState" class="form-control btn btn-primary">
                              <option selected>empleado</option>
                              <option>clave</option>
                              <option>clave</option>
                              <option>clave</option>
                           </select>
                        </div>
                     </form>
                  </nav>
               </li>
               <li v-for="task in searchEmployee" class="list-group-item"> {{task.empleado}}</li>
            </ul>
         </div>
      </div>
   </div>

</template>
<script>
   import axios from "axios"

   var urlEmployees = 'http://172.16.1.107:8000/api/cedis/1/employees'

   export default {
      name: 'Tasks',
      created: function(){
         this.getEmployees();
      },
      data () {
         return {
              tasks: [],
              employee: ''
         }
      },
      methods:{
         getEmployees: function(){
            axios.get(urlEmployees).then(response => {
               this.tasks = response.data.data;
            });
         }
      },
      computed:{
         searchEmployee: function(){
            return this.tasks.filter((item) => item.empleado.includes(this.employee.toUpperCase()));
         }
      }
   }

</script>
<style>
   .list-group-nav{
      list-style: none;
   }
</style> 