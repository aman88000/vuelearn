<template>
    <div>
        <h2>Props Parent Component vue js </h2>
        <ChildVue msg="From Parent static msg" :title="title"  v-on:changeTitle="updateTitle($event)"/>
    </div>
</template>

<script>
import ChildVue from './Child.vue'
    export default {
        name: 'ParentVue',
        data(){
            return {
                title: 'Parent title'
            }
        },
        components:{
            ChildVue
        },
        methods: {
            updateTitle(event){
                console.log('sfsfsfs', event)
            }
        }
    }
</script>

<style scoped>

</style>