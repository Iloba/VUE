<template>
    <div>
        <h1>Class Binding</h1>
        <h2 class="underline">Underlined Text</h2>
        <h2 class="underline" v-bind:class="status">Status</h2>
        <h2 v-bind:class="isPromoted && 'promoted'">Promoted</h2>
        <h2 v-bind:class="isSoldout ? 'sold-out' : 'new'">Sold out?</h2>
        <h2 v-bind:class="['new','promoted']">Newly Promoted Movie</h2>
        <h2 v-bind:class="[isPromoted && 'promoted', isSoldout ? 'sold-out' : 'new' ]">Array Conditional</h2>
        <h2 v-bind:class="{
            promoted: isPromoted,
            new: !isSoldout,
            'sold-out': isSoldout
        }">Object Conditional Movie</h2>

        <input type="text" placeholder="Enter Name" v-model="name" v-bind:class="name.length <= 5 ? 'red-border': 'green-border'"> <br>
        <span v-if="name.length >=5"  style="color:green;">Great</span>
        <span v-else style="color: red">This field is Required</span>

        

    </div>
</template>
<script>
export default {
   data(){
       return{
       status: 'danger', 
       isPromoted: true,
       isSoldout: false,
       name: '',
       inValid: true,
       Valid: false
    }
   }
   
}
</script>
<style scoped>
.underline{
    text-decoration: underline;
}
.danger{
    color: red;
}
.promoted{
    font-style: italic;
}
.new{
    color: greenyellow;
}

.sold-out{
    color: red;
}
.red-border{
    border: 1px solid red;
}
.green-border{
    border: 1px solid green;
}
.normal-border{
    border: 1px solid #eee;
}
</style>