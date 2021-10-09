<template>
    <h1>  {{ text }}</h1>
    <div v-html="h1 + h2">

    </div>
</template>
<script>
export default {
    data(){
        return{

            text: 'Emeka Iloba',
            h1: "<h1>Emeka Iloba </h1>",
            h2: "<h1>Kayettumi H Wakili</h1>"
        }
    }
}
</script>
<style scoped>

</style>