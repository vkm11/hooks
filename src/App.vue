<template>
  <div id="app">
    
    <created_beforeCreated />
    <Mount_beforeMount />
    <div v-if="display">
      <destroy_beforeDestroy />
    </div>
    <button v-on:click="toggle">Toggle</button>
  </div>
</template>

<script>
import created_beforeCreated from './components/created_beforeCreated.vue'
import Mount_beforeMount from './components/Mount_beforeMount.vue'
import destroy_beforeDestroy from './components/destroy_beforeDestroy.vue'
export default {
  name: 'App',
  components: {
    created_beforeCreated,
    Mount_beforeMount,
    destroy_beforeDestroy
  },
  data(){
    return{
      display:true
    }
  },
  methods:{
    toggle(){
      this.display=!this.display
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
