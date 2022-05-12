<template>
    <div>
        <h2>use of If, Else, for and show in vue </h2>
        <h4 v-if="total == 80">Topper</h4>
        <h4 v-else-if="total == 70">Good</h4>
        <h4 v-else>Avarage</h4>
        <h4 v-if="showData">show data using if</h4>
        <h4 v-show="showData">show data using show</h4>
        <h6 v-for="char in characters" :key="char"> {{char}}</h6>
        <ul>
            <li v-for="item in items" :key="item.id">{{item.id}}---- {{item.name}}</li>
        </ul>

    </div>
</template>

<script>
    export default {
        name: 'IfElseFor', 
        data(){
            return {
                total: 60,
                showData: true,
                characters: ['A', 'B', 'C'],
                items: [
                    {
                        id: 1,
                        name: 'aman'
                    },
                    {
                        id: 2,
                        name: 'Happy'
                    },
                    {
                        id: 3,
                        name: 'Rahul'
                    }
                ]
            }
        }
    }
</script>

<style scoped>

</style>