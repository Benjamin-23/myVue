<template>
    <label for="names">{{names}}</label>
    <input v-model="textvalue" :type="type" @change="lengthChecker()">
    <p v-if = "textlength < 8">{{errormsg}} {{textlength}}</p>

</template>
<script>
export default {
    name:"myInputs",
    props:{
        names: String,
        type: String
    },
    data(){
        return{
            textvalue:"",
            textlength:0,
            errormsg:"Too short"
        }
    },
    methods:{
        lengthChecker(){
            this.textlength ++
        console.log(this.textvalue)
            
        }
    }

}
</script>
<style>
    input{
        margin:10px 0px ;
        padding: 10px;
        width: 50%;
    }
    label{
        display: flex;
        flex-flow: column;

    }
</style>