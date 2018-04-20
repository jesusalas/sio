<template>
   <div id="app">
      <Tasks/>
   </div>
</template>

<script>
   import HelloWorld from './components/HelloWorld'
   import Login from './components/Login'
   import Employees from './components/Employees'
   import Tasks from './components/Tasks'

   export default {
      name: 'App',
      components: {
         HelloWorld,
         Login,
         Employees,
         Tasks
     }
   }
</script>

<style>
   #app {
      font-family: 'Avenir', Helvetica, Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      text-align: center;
      color: #2c3e50;
      margin-top: 60px;
   }
</style>
