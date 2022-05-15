<template>
    <div>
        <h2>Form vue js</h2>
        <h3>{{fromData}}</h3>
        <form @submit="fromSubmit">
            <label>Name: </label><input type="text"  v-model="fromData.name"/>  <br /><br />
            <label>Status: </label>
            <select v-model="fromData.status">
                <option>yes</option>
                <option>No</option>
            </select> <br /><br/>
            <label>Gender: </label>
            <label for="male">Male</label> <input id="male" type="radio" value="male" name="gender" v-model="fromData.gender" />
            <label for="female">Female</label> <input id="female" type="radio" value="female" name="gender"  v-model="fromData.gender" /> <br /><br />
                <button type="sumit">Submit</button>
        </form>
    </div>
</template>

<script>
    export default {
        name: 'FormVue',
        data(){
            return {
                fromData:{
                    name: '',
                    status: '',
                    gender: ''
                }
            }
        },
        methods: {
            fromSubmit(e){
                e.preventDefault();
                console.log(this.fromData)
            }
        }
    }
</script>

<style scoped>

</style>