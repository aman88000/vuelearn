<template>
    <div>
        <h2>Computed property used in vue js</h2>
        <h3>{{firstName}}  {{lastName}}</h3>

        <h2>Computed Property</h2>
        <h3>{{fullName}}</h3>

        <button @click="setName('Happy Singh')">change name</button>    
            <!-- <p> 
                v directives 
                v-pre
                v-show
                V-once
                v-html
                </p> -->
    </div>
</template>

<script>
    export default {
        name: 'ComputedVue',
        data(){
            return {
                firstName: 'Aman',
                lastName: 'Deep'
            }
        },
        methods:{
            setName(value){
               this.fullName = value
            }
        },
        computed:{
            fullName: {
                get(){
                    return  'Mr.'  + this.firstName + ' ' + this.lastName    
                },
                set(value){
                const name = value.split(' ');
                this.firstName = name[0]
                this.lastName = name[1]
                }
            }
        }
    }
</script>

<style scoped>

</style>