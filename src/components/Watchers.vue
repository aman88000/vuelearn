<template>
<div>
    <h1>Watcher used in vue js and its properties like immediate and deep</h1>
    <h2>{{formData.name}}</h2>
    <button @click="changeName">Change name</button>
</div>
</template>

<script>
export default {
    name: 'WatchersVue',
    data() {
        return {
            formData: {

                name: 'aman'
            }
        }
    },
    methods: {
        changeName() {
            this.formData.name = 'Deep'
        }
    },
    watch: {
        formData: {
            handler(currValue, preValue) {
                console.log('called', currValue, preValue)
            },
            immediate: true,
            deep: true
        }

    }
}
</script>

<style lang="scss" scoped>

</style>
