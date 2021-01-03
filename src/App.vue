<template>
  <div id="app">
    <form v-on:submit.prevent="onSubmit">
      用户名:{{ user.name }},密码:{{ user.password }}
      <hr/>
      <label>
        <span>用户名</span>
        <input type="text"
               :value="user.name"
               @input="user.name = $event.target.value">
      </label>
      <label>
        <span>密码</span>
        <input type="password" v-model="user.password">
      </label>
      <button>登录</button>
    </form>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      user: {
        name: '',
        password: ''
      }
    }
  },
  methods: {
    onSubmit() {
      const {user: {name, password}} = this
      console.log(name, password);
    }
  }
}
</script>
