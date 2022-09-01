<template>
 

  <input type="text" v-model="website" placeholder="type your website name"/>
  <a v-bind:href="website">My Website </a>

  <h4 v-bind:class="{active:activeBackground}">I am heading or leading to</h4>
<input type="text" v-model="customProp"/>
  <h1 :style="{color:customProp}">I am heading or leading to</h1>

</template>

<script>
 // i mport HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data()
  {
    return {
      website:"https://www.google.com",
      activeBackground:true,
      customProp : ""
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.active 
{
  background: lightblue;
}
</style>
