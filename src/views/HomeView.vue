<template>
  <div class="section container">
    <form>
      <input type="file" id="image-input" accept="image/jpeg, image/png, image/jpg">
    <div id="display-image"></div>
    </form>
    
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'HomeView',
  data()
  {
    return {
      website:"https://www.google.com",
      activeBackground:true,
      customProp : ""
    }},
  components: {
  // /  HelloWorld
  },
  methods:{

  },
  computed:{

  }
}


</script>

<style scoped>
  .section{

  }

  #display-image{
    width: 400px;
    height: 225px;
    border: 1px solid black;
    background-position: center;
    background-size: cover;
  }
</style>
