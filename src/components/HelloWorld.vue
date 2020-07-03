<template>
    <div>
      
      <h1>Counter App</h1>
      <p>{{count}}</p>

      <button v-on:click="count++">+</button>
      <button v-on:click="count=1">Reset</button>
      <button v-on:click="handleSubtract">-</button>
    </div>  
</template>

<script>
export default {
  name: 'CounterApp',
  data(){
    return {
      count: 1
    }
  },
  methods: {
    handleSubtract(){
      if(this.count > 1){
         return this.count--;
      }
    }
  }
  
}
</script>

