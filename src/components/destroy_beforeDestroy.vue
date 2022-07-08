<template>
    <div>
        <h1 style="color:darkmagenta">3. beforDestroy and Destroy in vuejs-2</h1>
        <h1>{{name}}</h1>
    </div>
</template>

<script>
export default {
    name: 'life-cycle_hooks',
    data()
    {
        return{
            name: "V-jai mane"
        }
    },
    beforeDestroy(){
        // you want to write anyting means you can use this component (ex: alert)
        alert("before") //first this conponent run 
        console.log('befor Destroyed')
    },
    destroyed(){
        alert("destroyed")
        console.log("destroyed")
    }
}
</script>

<style>

</style>