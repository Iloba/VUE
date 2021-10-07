<template>
    <div>
        This is Jude's Component
        {{ msg }}

            <br>

        <input type="text" v-model="inputText"> <br> <br>
        <textarea name="" id="" cols="30" rows="10" v-model="textlength"></textarea> <br>
        <span style="color: red;">{{textlength.length}}</span>
        <h2>{{inputText.length}}</h2>
    </div>
</template>
<script>
export default {
    props: ['msg'],
    data(){
        return{
            inputText: '',
            textlength: ''
        }
    }
}
</script>
<style scoped>

</style>