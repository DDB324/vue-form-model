<template>
  <div id="app">
    <div>爱好: {{ x }}</div>
    <label>
      <input type="checkbox" v-model="x" value="抽烟">
      <span>抽烟</span>
    </label>
    <label>
      <input type="checkbox" v-model="x" value="喝酒">
      <span>喝酒</span>
    </label>
    <label>
      <input type="checkbox" v-model="x" value="烫头">
      <span>烫头</span>
    </label>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      x: []
    }
  }
}
</script>
