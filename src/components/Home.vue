<template>
    <div>
        <h1>Home Component {{"helloi999".length}}  {{name}} <br/> {{phone}}</h1>
        <input type="file" v-model="input" /> {{input}}
        <span>
            {{getName("papa")}}
        </span>
        <h1>
            {{getData().name}}
        </h1>
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
            }
            
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
        }
    }
    
}

</script>
<style scoped>
    h1{
        color: green;
    }
</style>
