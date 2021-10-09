<template>
   
    <div :class="{hello:show, car:no}">
        Class Binding
    </div>
    <button @click="changeStyle()">Change Style</button>
    <button @click="addStyle()">Add Style</button>
</template>
<script>
export default {
    data(){
        return{

            show: true,
            no: false
          
            
        }
    },
    methods: {
        changeStyle(){
            this.show = !this.show;
        },
        addStyle(){
           this.no = true;
        }
    }
}
</script>
<style scoped>
    .hello{
        background: red;
    }
    .car{
        background: green;
    }
</style>