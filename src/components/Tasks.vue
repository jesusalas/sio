<template>
   
   <div class="container">
      <nav class="navbar navbar-dark bg-primary col-sm-6">
         <a class="navbar-brand" href="#">
            <form class="form-inline">
               <i class="material-icons">search</i>
               <input type="text" placeholder="Buscar" class="form-control btn-primary" v-model="employee">
               <i class="material-icons">account_circle</i>
            </form>
         </a>
      </nav>
      <nav class="navbar navbar-dark bg-dark col-sm-6">
         <a class="navbar-brand" href="#">
            <form class="form-inline">
               <i class="material-icons">arrow_back</i>
               <input type="text" placeholder="Buscar" class="form-control btn-none-color" v-model="employee">
               <i class="material-icons">close</i>
            </form>
         </a>
      </nav>
      <div class="row">
         <div class="col-sm-6">
            <ul class="list-group">
               <li class="list-none-line">
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
            </ul>
            <ul class="list-group list-container">
               <li v-for="task in searchEmployee" class="list-group-item"> 
               <ul>
                  <li class="list-none-line">{{ task.empleado }}</li>
                  <li class="list-none-line">{{ task.usuario}} - {{ task.contrasenia }}</li>
               </ul>
               </li>
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
   .list-none-line{
      list-style: none;
   }
   .list-container{
      max-height: 740px;
      overflow-y:scroll; 
   }
   .btn-none-color{
      background-color: transparent;
      border-color: transparent;
      color: white;
   }
   .btn-none-color:hover, .btn-none-color:focus, .btn-none-color::placeholder{
      background-color: transparent;
      border-color: transparent;
      color: white;
   }
   .btn-none-color::placeholder{
      color: #848484;
   }
</style> 