<template>
  <div>
     <h1 style="color:brown">1. beforCreated and created in vuejs-2</h1>
      <h1>{{name}}</h1>
  </div>
</template>

<script>
export default {
    name: 'life-cycle_hooks',
    data()
    {
        return{
            name: "vijay mane"
        }
    },
    created()
    {
        // in here name will be change becouse name should be already created
        this.name="Name changed kumar" 
        console.log("created", this.name);
    },
    beforeCreate()
    {
        // in here output name will be undefine not change 
        // this.name="Name changed kumar" // Undefined
        console.log("before",this.name)
    }
}
</script>

<style>

</style>