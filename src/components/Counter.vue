<template>
  <div>
    <h1>{{count}}</h1>
    <button v-on:click="addOne"> Add One </button>
    <button v-on:click="subtractOne"> Subtract One </button>
  </div>
</template>

<script>
export default {
  name:"Counter",
  data:function(){
      return {
          count:0,
      }
  },
  methods:{
    addOne:function(){
        console.log("Add was clicked")
        this.count++;
    },
    subtractOne:function(){
      console.log("Subtract was clicked")
      if (this.count > 0) {
        this.count--;
      }
    }
  }
}
</script>

<style scoped>
h1 {
  font-size: 70px;
  color: navy;
}
button {
  font-size: 16px;
  width: 10em;
  height: auto;
  margin: 2em;
}
</style>
