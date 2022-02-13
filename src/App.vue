<template>
  <Card :initValue=initValue @cardValueChange="cardValueChange"/>
</template>

<script>
import Card from "./components/Card.vue";

export default {
  name: "App",
  components: {
    Card,
  },
  data() {
    return {
      initValue: 10,
    };
  },
  methods:{
    cardValueChange(value){
      this.initValue = value
    }
  }
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0px;
  padding: 0px;
}
</style>
