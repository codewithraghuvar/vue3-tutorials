<template>
    <div class="full-border">
        <h1>Use Computed Porperty Second</h1>
        <input type="text" v-model="name"> 
        <template v-for="item in listItems" :key="item.id">
            <div>{{ item.name }}</div>
        </template>   
        <template v-for="item in list()" :key="item.id">
            <div>{{ item.name }}</div>
        </template>
        <div>
            totalItemPrice:  {{ totalItemPrice() }}
        </div>
        <div>
            total : {{ totalPrice }}
        </div>
        <button @click="items.push({id: '4',name: 'Computer',price: 300})">Add Item</button>
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
        name :'',
        items:[{
            id: '1',
            name: 'Laptop',
            price: 1000,

        },
        {
            id: '2',
            name: 'Mobile',
            price: 500,
        },
        {
            id: '3',
            name: 'Table',
            price: 300,
        }],
        finalArray: []

      }
    },
    computed :{
        listItems(){
            console.log('computed listItems call')
            return this.items
        },
        totalPrice() {
            return this.items.reduce((itemTotal, current) => (itemTotal = itemTotal + current.price), 0)
        }
    },
    methods: {
        
        list() {
            console.log('method list call')
            return this.items
        },
        totalItemPrice() {
            return this.items.reduce((itemTotal, current) => (itemTotal = itemTotal + current.price), 0)
        }
    }
  }
</script>
  
<style lang="scss">  
</style>
  