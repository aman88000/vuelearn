<template>
<!-- <BindStyle /> -->
<!-- <Methods /> -->
<!-- <IfElseFor /> -->
<!-- <Parent /> -->
<FormVue />
</template>

<script>
// import BindStyle from './components/BindStyle.vue'
// import Methods from './components/Methods.vue'
// import IfElseFor from './components/IfElseFor.vue'
// import Parent from "./components/props/Parent.vue"
import FormVue from "./components/Form/Form.vue"

export default {
  name: 'App',
  components: {
    // BindStyle,
    // Methods,
    // IfElseFor,
    // Parent,
    FormVue
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
