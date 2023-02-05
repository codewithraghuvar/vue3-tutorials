<template>
    <div class="full-border">
        <h1>Use methods</h1>
        <div> Name : {{ fullName }} </div>    
        <div>{{ getMessage() }}</div>
        <div>City : {{ getAddress().address }}</div>
        <div>City : {{ getAddress().city }}</div>
        <div>Pincode : {{ getAddress().pincode }}</div>
        <div>Address : {{ getAddress() }}</div>
    </div>
</template>
  
  <script>
  export default {
    name: 'HeaderComp',
    //declare varaible
    data (){
      return {
        fullName: 'Raghuvar Visht'
      }
    },
    methods: {
      getMessage(){
        return 'Welcome '+ this.fullName
      },
      getAddress() {
        return {
           address : 'Vikas Nagar',
           city: 'delhi',
           pincode: 110011
        }
      }
    }
  }
  </script>
  
  <style>
  
  </style>
  