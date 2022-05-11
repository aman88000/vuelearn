<template>
<h1>Home Component in vue </h1>
<p>{{name}}</p>
<p v-text="pText"></p>
</template>
<script>
export default{
    name: 'Home-vue',
    data(){
        return {
            name: 'Aman',
            pText: 'Testing for text added in p tag'

        }
    }
}
</script>
<style></style>