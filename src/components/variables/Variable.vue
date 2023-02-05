<template>
    <div class="full-border">
        <h1>Use variable</h1>
        <div> Name : {{ getFullName() }} </div>    
        <div>Age: {{ age }}</div>
        <div>New Age: {{ age==24}}</div>
        <div>Adult: {{ age===24}}</div>
        <div> Email : {{ email }} </div>
        <div> Pincode: <span v-text="pincode"></span></div>

    </div>
</template>
  
  <script>
  export default {
    name: 'HeaderComp',
    //declare varaible
    data (){
      return {
        firstName: 'Raghuvar',
        lastName: 'Visht',
        email: 'myemail@gmail.com',
        age: 18,
        pincode: 100111,
        getFullName () {
            return `${this.firstName} ${this.lastName}`
        }

      }
    }
  }
  </script>
  
  <style>
  
  </style>
  