<template>
  <div id="app">
    <HelloWorld v-bind:title="message" />
    <hr>
    <button class="btn btn-primary" v-on:click="doAction">change title</button>
    <Quiz quiz_text="test"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Quiz from './components/Quiz.vue'

export default{
  name:'App',
  components:{
    HelloWorld,
    Quiz
  },
  data(){
    return{
      message:'Hello',
    }
  },
  methods: {
    doAction(){
      var input = prompt("new title:")
      this.message = input
    }
  }
}

</script>


