<template>
<div>
    <h1>Watcher used in vue js and its properties like immediate and deep</h1>
    <h2>{{name}}</h2>
    <button @click="changeName">Change name</button>
</div>
</template>

<script>
export default {
    name: 'WatchersVue',
    data() {
        return {
            name: 'aman'
        }
    },
    methods: {
        changeName() {
            this.name = 'Deep'
        }
    },
    watch: {
        name: {
            handler(currValue, preValue) {
                console.log('called', currValue, preValue)
            },
            immediate: true
        }

    }
}
</script>

<style lang="scss" scoped>

</style>
