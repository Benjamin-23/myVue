<template>
  <div class="hello">
    <h5>{{msg}}</h5>
    <!-- register form with all details -->
    <div class="form-cointainer">
      <form action="">
        <myInputs type="text"/>
        <myInputs names="Email" type="email"/>
        <myInputs names="number" type="number"/>
    
    
      </form>
    </div>

    
  </div>


</template>

<script>
import myInputs from "../components/myInputs.vue";

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components:{
    myInputs

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
