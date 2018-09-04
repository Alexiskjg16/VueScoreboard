<template>
  <div id="app">
    <section>
    <h1> JayHawks </h1>
    <h2> Home Team </h2>
    <Counter />
  </section>
  <div>
    <Sessions />
  </div>
  <section>
    <PlayerName />
    <h2> Visiting Team </h2>
    <Counter />
  </section>
  </div>
</template>

<script>
import PlayerName from './components/PlayerName.vue'
import Counter from './components/Counter.vue'
import Sessions from './components/Sessions.vue'

export default {
  name: 'app',
  components: {
    PlayerName,
    Counter,
    Sessions
  }
}
</script>

<style scope>
#app {
  display: flex;
  font-family: Avenir, 'Helvetica', Arial, sans-serif;
  text-align: center;
  justify-content: space-around;
  color: #2c3e50;
  background-color:blue;
  height: 100%;
}
section {
  border: 1px solid black;
  background-color: white;
  width: 25em;
}
h1 {
  font-size: 50px;
  color: red;
  border: 1px solid black;
}
button {
  background-color: red;
  width: 7em;
  height: 8em;
}
</style>
