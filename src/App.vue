<template>
  <h1>Method Properties</h1>
  <p>Variable {{var1}}</p>
  <p>Variable {{var2}}</p>
  <input type="number" name="" v-model="pass">
  <p>{{var1}} * {{var2}} * {{pass}} = {{functionMethon(pass)}}</p>
  <input type="number" name="" v-model="principal">
  <input type="number" name="" v-model="rate">
  <input type="number" name="" v-model="time">

  <p> principal {{principal}} * rate {{rate}} *  time {{time}} /100= {{simpleInterest}}</p>

  

</template>

<script>
 // i mport HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data(){
   return{
    var1:10,
    var2:20,
    pass:"",
    principal:"",
rate:"",
time:"",
   }
  },
  components: {
    // HelloWorld
  },
methods:
{
  functionMethon(pass)
  {
    return this.var1* this.var2 *pass
  }
},computed:
{
 simpleInterest()
  {
    return this.principal* this.rate *this.time/100;
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
</style>
