<template>
    <div class="form-container">
        {{ JSON.stringify(formValues) }}
        <div>
            <label for="name">Name</label>
            <input type="text" id="name" v-model="formValues.name"/>
        </div>
        <div>
            <label for="profile">Profile Summary</label>
            <textarea  id="profile" v-model="formValues.profileSummary">
            </textarea>
        </div>

    </div>
</template>
<script>
export default {
    name : 'UserForm',
    data() {
        return {
            formValues :{
                name: '',
                profileSummary: '',

            }
        }
    }
}
</script>
<style>
</style>