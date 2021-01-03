<template>
  <div class="wrapper">
    <input :value="value" @input="onInput">
  </div>
</template>

<script>
export default {
  name: 'MyInput',
  props:{
    value:{
      type:String,
    }
  },
  methods: {
    onInput(e) {
      this.$emit('input', e.target.value)
    }
  }
}
</script>

<style>
.wrapper {
  border: 1px solid red;
  display: inline-block;
}
</style>