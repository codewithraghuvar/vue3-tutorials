<template>
    <h1 class="header">
      This is header
      {{ "header".length }}
     <div> Email : {{ email }} </div> 
    </h1>
  </template>
  
  <script>
  export default {
    name: 'HeaderComp',
    components: {
      
    },
    data (){
      return {
        email: 'myemail@gmail.com'
      }
    }
  }
  </script>
  
  <style>
  .header {
    color: red
  }
  </style>
  