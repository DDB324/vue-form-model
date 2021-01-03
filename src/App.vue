<template>
  <div id="app">
    <div>你想做: {{ x }}</div>
    <label>
      <input name="want" type="radio" v-model="x" value="抽烟">
      <span>抽烟</span>
    </label>
    <label>
      <input name="want" type="radio" v-model="x" value="喝酒">
      <span>喝酒</span>
    </label>
    <label>
      <input name="want" type="radio" v-model="x" value="烫头">
      <span>烫头</span>
    </label>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      x: ''
    }
  }
}
</script>
