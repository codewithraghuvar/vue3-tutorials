<template>
    <div class="full-border">
        <h1>Use Computed Porperty</h1>
        <div>First Name : <input type="text" v-model="firstName"></div>
        <div>Computed  Name : {{ fullName }} </div> 
        <div>Method  Name : {{ getName() }} </div>    
        <div>Country : <input type="text" v-model="country"></div>
        
    </div>
</template>
  
  <script>


  export default {
    name: 'ComputedProperty',
    //declare varaible
    data (){
      return {
        firstName: 'Raghuvar',
        lastName: 'Visht',
        country :'',

      }
    },
    computed :{
        fullName(){
            console.log('computed fullName')
            return this.firstName + this.lastName
        }
    },
    methods: {
        getName() {
            console.log('method getName')
            return this.firstName + this.lastName
        }
    }
  }
  </script>
  
  <style lang="scss">
  
  </style>
  