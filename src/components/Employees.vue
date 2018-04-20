<template>
   <div class="container">
      <form>
         <div class="form-group row">
            <label for="idEmployeInputText" class="col-sm-2 col-form-label">ID Empleado:</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="idEmployeInputText">
            </div>
            <div class="col-sm-2">
               <button class="btn btn-primary">Buscar</button>
            </div>
            <label for="findEmployeeButton" class="col-sm-2 col-form-label">Clave Contable: *</label>
            <div class="col-sm-4">
               <input type="text" class="form-control" id="findEmployeeButton">
            </div>
         </div>
         <div class="form-group row">
            <label for="nameInputText" class="col-sm-2 col-form-label">Nombre: *</label>
            <div class="col-sm-10">
               <input type="text" class="form-control" id="nameInputText">
            </div>
         </div>
         <div class="form-group row">
            <label for="lastNameInputText" class="col-sm-2 col-form-label">Apellido Paterno: *</label>
            <div class="col-sm-4">
               <input type="text" class="form-control" id="lastNameInputText">
            </div>
            <label for="surnameInputText" class="col-sm-2 col-form-label">Apellido Materno: *</label>
            <div class="col-sm-4">
               <input type="text" class="form-control" id="surnameInputText">
            </div>
         </div>
         <div class="form-group row">
            <label for="streetInputText" class="col-sm-2 col-form-label">Calle: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="streetInputText">
            </div>
            <label for="streetNumberInputText" class="col-sm-2 col-form-label">Numero: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="streetNumberInputText">
            </div>
            <label for="SuburbInputText" class="col-sm-2 col-form-label">Colonia: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="SuburbInputText">
            </div>
         </div>
         <div class="form-group row">
            <label for="cityInputText" class="col-sm-2 col-form-label">Ciudad: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="cityInputText">
            </div>
            <label for="stateInputText" class="col-sm-2 col-form-label">Estado: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="stateInputText">
            </div>
            <label for="codeZipTextBox" class="col-sm-2 col-form-label">Codigo Postal: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="codeZipTextBox">
            </div>
         </div>
         <div class="form-group row">
            <label for="telephoneNumberInputText" class="col-sm-2 col-form-label">Telefono: </label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="telephoneNumberInputText">
            </div>
            <label for="emailInputText" class="col-sm-2 col-form-label">Email: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="emailInputText">
            </div>
            <label for="typeBloodInputText" class="col-sm-2 col-form-label">Tipo de Sangre: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="typeBloodInputText">
            </div>
         </div>
         <div class="form-group row">
            <label for="" class="col-sm-2 col-form-label">RFC: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="">
            </div>
            <label for="" class="col-sm-2 col-form-label">CURP: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="">
            </div>
            <label for="" class="col-sm-2 col-form-label">IMSS: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="">
            </div>
         </div>
         <div class="form-group row">
            <label for="entranceHourInputText" class="col-sm-2 col-form-label">Entrada Matutina: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="entranceHourInputText">
            </div>
            <label for="" class="col-sm-2 col-form-label">Entrada Vespertina: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="">
            </div>
            <label for="" class="col-sm-2 col-form-label">Empresa: *</label>
            <div class="col-sm-2">
               <input type="text" class="form-control" id="">
            </div>
         </div>
         <div class="form-group row">
            <label for="" class="col-sm-2 col-form-label">Área: *</label>
            <div class="col-sm-4">
               <input type="text" class="form-control" id="">
            </div>
            <label for="" class="col-sm-2 col-form-label">Departamento: *</label>
            <div class="col-sm-4">
               <input type="text" class="form-control" id="">
            </div>
         </div>
         <div class="form-group row">
            <label for="" class="col-sm-2 col-form-label">Sub Área: *</label>
            <div class="col-sm-4">
               <input type="text" class="form-control" id="">
            </div>
            <label for="" class="col-sm-2 col-form-label">Puesto: *</label>
            <div class="col-sm-4">
               <input type="text" class="form-control" id="">
            </div>
         </div>
         <div class="form-group row">
            <label for="" class="col-sm-2 col-form-label">Cedis: *</label>
            <div class="col-sm-4">
               <input type="text" class="form-control" id="">
            </div>
            <label for="" class="col-sm-2 col-form-label">Tipo Empleado: *</label>
            <div class="col-sm-4">
               <input type="text" class="form-control" id="">
            </div>
         </div>
         <div class="form-group row">
            <label for="" class="col-sm-2 col-form-label">Limite Credito:</label>
            <div class="col-sm-8">
               <input type="text" class="form-control" id="">
            </div>
         </div>
         <div class="form-group row">
            <label for="" class="col-sm-2 col-form-label">Usuario:</label>
            <div class="col-sm-4">
               <input type="text" class="form-control" id="">
            </div>
            <label for="" class="col-sm-2 col-form-label">Contraseña:</label>
            <div class="col-sm-4">
               <input type="text" class="form-control" id="">
            </div>
         </div>
         <div class="form-group row">
            <label for="" class="col-sm-2 col-form-label">Confirmar Contraseña:</label>
            <div class="col-sm-8">
               <input type="text" class="form-control" id="">
            </div>
         </div>
         <div class="form-group row">
            <div class="col-sm-12">
               <button class="btn btn-primary">Guardar</button>
               <button class="btn btn-primary">Desactivar</button>
               <button class="btn btn-primary">Limpiar</button>
               <button class="btn btn-primary">Biometrica</button>
               <button class="btn btn-primary">Foto</button>
               <button class="btn btn-primary">Salir</button>
            </div>
         </div>        
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