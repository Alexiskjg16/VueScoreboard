<template>
  <div class="hello">
    <h1>{{nameDisplay}}</h1>
    <input type="text" placeholder="Name Here" v-model="playerName" />
    <button v-on:click="inputName">Change Team Name </button>
  </div>
</template>

<script>
export default {
  name: 'playerName',
  data:function(){
    return {
    playerName:"",
    nameDisplay: "OpposingTeam"
  }
},
methods:{
  inputName : function(){
    this.nameDisplay = this.playerName
  }
 }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  border: 1px solid black;
  font-size: 50px;
  color: red;
}
button {
  background-color: white;
  font-size: 16px;
  width: 10em;
  height: auto;
  margin: 2em;
}
</style>
