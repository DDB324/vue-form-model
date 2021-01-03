<template>
  <div id="app">
    <input placeholder="edit me" v-model="message">
    <p>Message is: {{message}}</p>
    <p><button @click="message = 'ddb'">set message to ddb</button></p>
  </div>
</template>

<script>

export default {
  name: 'App',
  data(){
    return {
      message:'hi'
    }
  }
}
</script>
