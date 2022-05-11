<template>
    <div>
        <h2>How to use Methods in vue js </h2>
        <h3>{{name}}</h3>
        <h4>{{getName('aman')}}</h4>
        <button v-on:click="changeName">Change Name</button>
        <div v-on:mouseover="overChange">On mouse Hover</div>
        <button v-on:click="setName('Happy', $event)">set Name</button>
        <button @click="setName('Happy', $event)">set Name</button>
    </div>
</template>

<script>
    export default {
        name: 'Methods-vue',
        data(){
            return {
                name: 'aman'
            }
        },
        methods: {
            getName(name){
                return 'methods called ' + name
            },
            changeName(event){
                console.log(event)
                this.name = 'Deep'
            },
            overChange(){
                console.log('yes')
            },
            setName(name, event){
                this.name = name;
                console.log(event)
            }
        }
    }
</script>

<style scoped>

</style>