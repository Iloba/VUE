<template>
    <div>
        <h1>Home Component {{"helloi999".length}}  {{name}} <br/> {{phone}}</h1>
        <input type="text" v-model="input" /> {{input}}
        <span>
            {{getName("papa")}}
        </span>  <br>
        <h1>
            {{getData().name}}
        </h1>
        <button v-on:click="buttonClick()">Click ME</button>
        <button v-on:dblclick="buttonClick()">Double Click ME</button>
        <h2>{{count}}</h2>
        <button @click="increaseCount()">Increase Count</button>
        <button @click="decreaseCount()">Decrease Count</button>
    </div>
</template>
<script>
export default{
    name: "Home",
    data(){
        return{
            input: '',
            name: 'EmekaSney',
            phone: 18054421788,
            getName(x){
                return x;
            },
            count: 1
            
        }
    },
    methods:{
        getNames(){
            return "Bro B";
        },
        getData(){
            return {
                name: this.name,
                age: 12,
                class: "100 Level",
            }
        },
        buttonClick(){
             alert(this.getData().name);
        },
        increaseCount(){
            this.count++;
        },
        decreaseCount(){
            this.count--;
        }
    }
    
}

</script>
<style scoped>
    h1{
        color: green;
    }
</style>
