<template>
   <div>
      <p v-if="hasPermissions" class="message-success">Todo se encuentra en orden</p>   
      <p v-else class="message-failed">Se encontraron uno o mas errores en tu cuenta</p>
   </div>
</template>

<script>
   export default {
      name: 'Login',
      data: ()=> ({ 
            hasPermissions: false
      })
   }
</script>

<style>
   .message-success{
      color: blue;
   }
   .message-failed{
         color: red;
      }
</style>