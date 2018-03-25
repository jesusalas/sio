<template>
   <div>
      <form>
         <div class="row justify-content-md-center">
            <div class="form-group col col-md-4">
               <label for="exampleInputEmail1">Email address</label>
               <input type="email" class="form-control" id="exampleInputEmail1" aria-describedby="emailHelp" placeholder="Enter email">
               <small id="emailHelp" class="form-text text-muted">We'll never share your email with anyone else.</small>
            </div>
            <div class="form-group col col-md-4">
               <label for="exampleInputPassword1">Password</label>
               <input type="password" class="form-control" id="exampleInputPassword1" placeholder="Password">
            </div>
         </div>
         <div class="row">
            <div class="col col-md-8">
               1 of 3
            </div>
         </div>
         
        <div class="form-check">
          <input type="checkbox" class="form-check-input" id="exampleCheck1">
          <label class="form-check-label" for="exampleCheck1">Check me out</label>
        </div>
        <button type="submit" class="btn btn-primary">Submit</button>
      </form>
      <form action="">
         <label for="idEmployeeTextBox">ID Empleado:</label>
         <input type="text" id="idEmployeeTextBox">
         <label for="">Clave Contable: *</label>
         <input type="text">
         <label for="">Nombre: *</label>
         <input type="text">
         <label for="">Apellido Paterno: *</label>
         <input type="text">
         <label for="">Apellido Materno: *</label>
         <input type="text">
         <label for="">Calle: *</label>
         <input type="text">
         <label for="">Numero: *</label>
         <input type="text">
         <label for="">Colonia: *</label>
         <input type="text">
         <label for="">Ciudad: *</label>
         <input type="text">
         <label for="">Estado: *</label>
         <input type="text">
         <label for="">Codigo Postal: *</label>
         <input type="text">
         <label for="">Telefono: </label>
         <input type="text">
         <label for="">Email: *</label>
         <input type="text">
         <label for="">Tipo de Sangre: *</label>
         <input type="text">
         <label for="">RFC: *</label>
         <input type="text">
         <label for="">CURP: *</label>
         <input type="text">
         <label for="">IMSS: *</label>
         <input type="text">
         <label for="">Entrada Matutina: *</label>
         <input type="text">
         <label for="">Entrada Vespertina: *</label>
         <input type="text">
         <label for="">Empresa: *</label>
         <input type="text">
         <label for="">Área: *</label>
         <input type="text">
         <label for="">Departamento: *</label>
         <input type="text">
         <label for="">Sub Área: *</label>
         <input type="text">
         <label for="">Puesto: *</label>
         <input type="text">
         <label for="">Cedis: *</label>
         <input type="text">
         <label for="">Tipo Empleado: *</label>
         <input type="text">
         <label for="">Limite Credito:</label>
         <input type="text">
         <label for="">Usuario:</label>
         <input type="text">
         <label for="">Contraseña:</label>
         <input type="text">
         <label for="">Confirmar Contraseña:</label>
         <input type="text"> 
      </form>
   </div>
</template>

<script>
   export default {
      name: 'Employees',
      data () {
         return {
            miMensajeGenial: 'Soy una verga con Vue',
            flag: true
         }
      }
   }
</script>

<style>
   .message-success{
      color: blue;
   }
</style>