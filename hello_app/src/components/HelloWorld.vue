<template>
  <div class="alert alert-info">
    <h2>{{ title }}</h2>
    <p>{{ message }}</p>
    <hr>
    <div>
      <input type="text" class="form-control" v-model="input">
      <button class="btn btn-info mt-2" v-on:click="doAction">Click</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    title: String,
    message: String,
  },
  data() {
    return {
      message: 'お名前は？',
      input: 'no name',
    }
  },
  methods: {
    doAction() {
      this.message = 'こんにちは、' + this.input + 'さん！'
    }
  }
}
</script>

