<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <!-- <HelloWorld msg="Welcome to Your Vue.js + TypeScript App"/> -->
    <div>{{ msg }}</div>
    <div v-for="item of list" :key="item">
      {{item}}
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent, reactive, ref } from 'vue'

// export default class Home extends Vue {
export default defineComponent({
  name: 'App',
  setUp() {
    const msg = ref('aaa')
    const list = ref(['1', '2', '3'])
    return {list,msg}
  }
})
</script>
