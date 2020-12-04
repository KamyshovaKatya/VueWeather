<template>
  <div id="app">
    <div class="informer-container">
        <Temperature></Temperature>
        <Humidity></Humidity>
        <Wind></Wind>
    </div>
  </div>
</template>

<script>
import Temperature from './components/temp.vue'
import Wind from './components/wind.vue'
import Humidity from './components/humidity.vue'

export default {
  name: 'App',
  components: {
    Temperature, Wind, Humidity
  }
}
</script>

<style>
#app {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background: rgb(244, 123, 186);
  background: linear-gradient(-25deg, rgba(244, 123, 186, 0.5) 20%, rgba(90, 95, 245, 0.5) 80%);
}

.informer-container {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-wrap: wrap;
  width: 400px;
  padding: 30px;
  background-image: url('assets/forest.png');
  background-size: cover;
  background-position: center center;
  border-radius: 20px;
  box-shadow: 0px 0px 10px 0px rgba(50, 50, 50, 0.75);
}
</style>
