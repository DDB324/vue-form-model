<template>
  <div id="app">
    <select v-model="x">
      <option value="" disabled>请选择</option>
      <option :value="item.text" v-for="item in array" :key="item.value">
        {{ item.text }}
      </option>
    </select>
    <hr/>
    <div>
      <span>x : {{ x }}</span>
    </div>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      array: [
        {text: '抽烟', value: 1},
        {text: '喝酒', value: 2},
        {text: '烫头', value: 3}
      ],
      x: ''
    }
  }
}
</script>
