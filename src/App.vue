<template>
   <div id="app">
      <Login/>
      <Employees/>
   </div>
</template>

<script>
   import HelloWorld from './components/HelloWorld'
   import Login from './components/Login'
   import Employees from './components/Employees'

   export default {
      name: 'App',
      components: {
         HelloWorld,
         Login,
         Employees
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
