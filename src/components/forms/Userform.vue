<template>
    <div>
        {{ JSON.stringify(formValues) }}
        <form >
            <div>
            <label for="fname">Name</label>
            <input type="text" id="fname" v-model.trim="formValues.name" placeholder="Your name..">
            </div>
            <div>
                <label> Gender</label>
                <input type="radio" id="man" value="men" v-model="formValues.gender"/>   
                <label for="man">Men</label>
                <input type="radio" id="women" value="women" v-model="formValues.gender"/>   
                <label for="women">Women</label>                
            </div>
            <div>
                <label for="fname">Age</label>
                <input type="number" id="age" max-value="150" v-model.number="formValues.age" >
            </div>
            <div>
            <label for="country">Country</label>
            <select id="country" v-model="formValues.country">
                <option value="">Select country</option>
                <option value="australia">Australia</option>
                <option value="canada">Canada</option>
                <option value="usa">USA</option>
            </select>
            </div>
            <div>
                <input type="checkbox" id="remoteWork" v-model="formValues.remoteWork" 
                    true-value="yes" false-value="no"/>   
                <label for="remoteWork">Open to a remove work</label>
            </div>
            <div>
                <label> Skills</label>
                <input type="checkbox" id="skillJava" value="java" v-model="formValues.skillSet"/>   
                <label for="skillJava">Java</label>
                <input type="checkbox" id="skillpython" value="python" v-model="formValues.skillSet"/>   
                <label for="skillpython">Python</label>
                <input type="checkbox" id="skilljavascript" value="javascript" v-model="formValues.skillSet"/>   
                <label for="skilljavascript">JavaScript</label>
            </div>
            <div>
                <label for="summary"> Summary </label>
                <textarea id="summary" v-model="formValues.summary"></textarea>
            </div>

            <button v-on:click="save($event)">Save</button>
        </form>
</div>

</template>
<script>
export default {
    name : 'UserForm',
    data() {
        return {
            formValues: {
                name: '',
                summary: '',
                gender: '',
                age: '',
                country: '',
                jobLocation:[],
                remoteWork: false,
                skillSet :[]
            }
        }
    },
    methods:{
      save(event){
        event.preventDefault()
        console.log('formValues=='+JSON.stringify(this.formValues))
      }
    }
}
</script>
<style lang="scss">
input[type=text],input[type=number] , select{
  width: 100%;
  padding: 12px 20px;
  margin: 8px 0;
  display: inline-block;
  border-radius: 4px;
  box-sizing: border-box;
}
input[type=text],input[type=number], select {
 border: 1px solid #ccc;
}
input[type=submit] {
  background-color: #4CAF50;
  color: white;
  cursor: pointer;
  &:hover {
    background-color: #45a049;
  }
  
}

div {
  border-radius: 5px;
  background-color: #f2f2f2;
  padding: 5px;
}

</style>