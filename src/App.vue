<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
    <div>ssss</div>
    <div>{{msg}}</div>
    <div v-for="item of list" :key="item">
      {{item}}
    </div>
    <section>
            <video src="blob:https://jx.123ku.com/f28b565d-6ccb-4d50-9640-3f752be02db1"></video>
        <video class="dplayer-video dplayer-video-current" webkit-playsinline="" x-webkit-airplay="allow" playsinline="" preload="metadata" src="blob:https://jx.123ku.com/202d1755-f186-4bed-bfce-cf143d414927"></video>
    </section>
    <section>
      <a href="blob:https://jx.123ku.com/202d1755-f186-4bed-bfce-cf143d414927">download</a>
    </section>
    <router-view/>
  </div>
  <!-- <router-view/> -->
</template>

<script lang="ts">
import { defineComponent, reactive, ref } from 'vue'

// export default class Home extends Vue {
export default defineComponent({
  name: 'App',
  setUp() {
    const msg = ref('aaa')
    const list = ref(['1', '2', '3'])
    return {
      list,
      msg
    }
  }
})
</script>

<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
