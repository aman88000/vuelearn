<template>
    <div>
<h2>child props Component vue js </h2>
<h3>{{msg}}--- {{title}}</h3>
<button v-on:click="setTitle">set Title</button>
    </div>
</template>

<script>
    export default {
        name: 'ChildVue',
        props: [
            'msg',
            'title'
        ],
        methods: {
            setTitle(){
                console.log('yesy')
                this.$emit('changeTitle', 'updated title from child using emit')
            }
        }
    }
</script>

<style scoped>

</style>