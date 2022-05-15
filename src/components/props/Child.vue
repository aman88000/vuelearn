<template>
    <div>
<h2>child props Component vue js </h2>
<h3 v-bind="$attrs">{{msg}}--- {{title}}</h3>
<button v-on:click="setTitle">set Title</button>
    </div>
</template>

<script>
    export default {
        name: 'ChildVue',
        // props: [
        //     'msg',
        //     'title'
        // ],
        props: {
            msg: String,
            title: String
        },
        methods: {
            setTitle(){
                console.log('yesy')
                this.$emit('changeTitle', 'updated title from child using emit')
            }
        },
        inheritAttrs: false
    }
</script>

<style scoped>

</style>