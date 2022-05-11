<template>
<h1>Home Component in vue </h1>
<p>{{name}}</p>
<p v-text="pText"></p>
<p v-html="pHtml"></p>
<h3 v-bind:id="headingID">Heading h3</h3>
<button v-bind:disabled="flag">Disable or enable</button>
<p v-bind:class="active" class="abc">Active</p>
<p v-bind:class="isLogin && 'login'">Login class</p>
<p v-bind:class="isLogin ? 'login': 'logout'">Login/Logout</p>
<p v-bind:class="[isLogin && 'class1', 'class2']">Array classes</p>
<p v-bind:style="{
    color: 'red',
    fontSize: '20px'
}">Style added inline</p>

<p v-bind:style="{
    color: 'red',
    'font-size': '30px'
}">Style added inline</p>

<p v-bind:style="styleObj1">Style obj used</p>
<p v-bind:style="styleObj1">Style multiple obj used</p>
<p v-bind:style="[styleObj1, styleObj2]">Style multiple obj used</p>
</template>
<script>
export default{
    name: 'Home-vue',
    data(){
        return {
            name: 'Aman',
            pText: 'Testing for text added in p tag',
            pHtml: '<h3>Hello Testing Added H3 html tag</h3>',
            headingID: 'Header-id',
            flag: true,
            active: 'active-class',
            isLogin: false,
            styleObj1: {
                 color: 'red'
            },
            styleObj2: {
                    'font-size': '30px'
            }


        }
    }
}
</script>
<style></style>