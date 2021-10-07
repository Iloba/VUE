<template>
    <div>
        <h1>Please Select your Skills</h1>
        <label for="PHP">Php</label>
        <input type="checkbox" id="PHP" v-model="tech" value="PHP">


         <label for="Laravel">Laravel</label>
        <input type="checkbox" id="Laravel" v-model="tech" value="Laravel">

        <label for="Bootstrap">Bootstrap</label>
        <input type="checkbox" id="Bootstrap" v-model="tech" value="Bootstrap">

        <h3>{{tech}}</h3>

        <label for="student">Student</label>
        <input type="radio"  id="student" value="student" v-model="proffession">

         <label for="developer">Developer</label>
        <input type="radio"  id="developer" value="developer"  v-model="proffession">


        <br> 

        <h2>I am a: {{proffession}}</h2>
    </div>
</template>
<script>
export default {
    data(){
        return{
            tech: [],
            proffession: null
        }
    }
}
</script>
<style scoped>

</style>