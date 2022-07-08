<template>
  <div>
      <h1 style="color:peru">2. BeforeMount and Mounted in vuejs-2</h1>
      <h1 id="demo">{{name}}</h1>
  </div>
</template>

<script>
export default {
    name: "Mount_beforeMount",
    data(){
        return{
            name:"Vijaykumar Mane"
        }
    },
    // when you modify the html DOM that time we can use 
    beforeMount(){
        // first call beforeMount 
        // here we can't modify the dom
        console.log('beforemount',document.getElementById('demo'));
    },
    mounted(){
        // here we can modify the dom 
        console.log('mounted',document.getElementById('demo'))
    }
}
</script>

<style>

</style>