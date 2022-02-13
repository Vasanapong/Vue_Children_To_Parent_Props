<template>
  <div class="card">{{initValue}}</div>
  <button @click="cardValueChange()">Change Value</button>
</template>

<script>
export default {
    name:"Card",
    props:{
        initValue:Number
    },
    methods:{
        cardValueChange(){
            this.$emit('cardValueChange',this.initValue+10)
        }
    },
    emits:["cardValueChange"]
}
</script>

<style>

</style>