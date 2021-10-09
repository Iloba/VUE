<template>
        <Html/>
    <div>
       
        {{ data    }} <br>
        
      
         <ul>
             <li v-for="friend in friends" :Key="friend">{{friend}}</li>
        </ul>
        <ul>
            <li v-for="user in users" :key="user">
                {{ user.name }}, {{ user.class }}, {{ user.age }} School: {{ user.school }}
            </li>
        </ul>
    </div>
</template>
<script>
import Html from './Html.vue'
export default {
    props: {
        'data': String, 
        'getData':Function
    },
    components:{
        Html
    },
    data(){
        return{
            friends: ['emeka', 'jude', 'kaye', 'sney'],
            users: [
                {
                    name: 'Emeka',
                    class: '200 Level',
                    age: '18',
                    school: {
                        yearOne: 'Afit',
                        yearTwo: 'Afit',
                        yearThree: 'Abuja'
                    },
                      
                    
                },

                 {
                    name: 'Kaye',
                    class: '100 Level',
                    age: '18',
                    school: {
                        yearOne: 'Afit',
                        yearTwo: 'Afit',
                        yearThree: 'Abuja'
                    },
                },
                 {
                    name: 'Jude',
                    class: '100 Level',
                    age: '19',
                    school: {
                        yearOne: 'Afit',
                        yearTwo: 'Afit',
                        yearThree: 'Abuja'
                    },
                },

            ]
        }
    },
    methods:{
         getDatas(){
             alert('hello');
         }
    }
}
</script>
<style scoped>

</style>