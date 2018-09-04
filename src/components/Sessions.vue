<template>
<div>
<h1> Quarter </h1>
<button v-for="q in quarters" v-bind:class="{currentQuarter: quarter === q}" v-on:click="() => updateQuarter(q)">{{q}}</button>
</div>
</template>

<script>
export default {
  name: "Sessions",
  data:function(){
    return {
      testing:true,
      quarter: 0,
      quarters: [1,2,3,4]
    }
  },
  methods:{
    updateQuarter: function(q){
      this.quarter = q
    }
  }

}
</script>

<style scoped>
 .currentQuarter{
   background-color:navy;
 }
 h1 {
   background-color: white;
 }
</style>
