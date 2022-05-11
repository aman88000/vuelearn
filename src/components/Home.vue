<template>
<h1>Home Component in vue </h1>
<p>{{name}}</p>
<p v-text="pText"></p>
<p v-html="pHtml"></p>
</template>
<script>
export default{
    name: 'Home-vue',
    data(){
        return {
            name: 'Aman',
            pText: 'Testing for text added in p tag',
            pHtml: '<h3>Hello Testing Added H3 html tag</h3>'

        }
    }
}
</script>
<style></style>