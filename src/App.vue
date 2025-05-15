<script setup>
import { createApp } from 'vue'
import HelloWorld from './components/HelloWorld.vue'
console.log(HelloWorld)
const helloWorldFnc = () => {
  // console.log('helloWorldFnc')
  // const el = document.createElement('div')
  // const instance = createApp(HelloWorld, { msg: 'Vite + Vue',  modelValue: true,
  //   'onUpdate:modelValue': (val) => {
  //     if (!val) el.remove()
  //   } })
  // // instance.vm = instance.$mount()
  // //  this.$el.appendChild(instance.vm.$el)
  // // app.dialogVisible = true
  // // console.log(app)
  // // debugger
  // instance.mount(el)
  // document.body.appendChild(el)
  // HelloWorld.setup()
  // HelloWorld.render()

}
// const 
</script>

<template>
  <!-- <HelloWorld msg="3333" /> -->
  <el-button type="primary" @click="helloWorldFnc()">创建一个组件</el-button>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
