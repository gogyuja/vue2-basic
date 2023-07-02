<template>
  <header>
    <h1>{{propsdata}}
      <button v-on:click="sendEvent">send</button>
    </h1>
  </header>
</template>

<script>
export default {
  props:['propsdata'],
  methods:{
    sendEvent:function(){
      this.$emit('renew');
    }
  }
}
</script>

<style>

</style>