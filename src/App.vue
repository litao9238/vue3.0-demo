<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
  <router-view/>
</template>

<script>
import { onBeforeMount, onMounted, onBeforeUpdate, onUpdated, onBeforeUnmount, onUnmounted, onActivated, onDeactivated, onErrorCaptured } from'vue'

export default {
  setup() {
    console.warn('app setup')
    onBeforeMount(() => {
      console.log('onBeforeMount')
      // ...
    })
    onMounted(() => {
      console.log('onMounted')
      // ...
    })
    onBeforeUpdate(() => {
      console.log('onBeforeUpdate')
      // ...
    })
    onUpdated(() => {
      console.log('onUpdated')
      // ...
    })
    onBeforeUnmount(() => {
      console.log('onBeforeUnmount')
      // ...
    })
    onUnmounted(() => {
      console.log('onUnmounted')
      // ...
    })
    onActivated(() => {
      console.log('onActivated')
      // ...
    })
    onDeactivated(() => {
      console.log('onDeactivated')
      // ...
    })
    onErrorCaptured(() => {
      console.log('onErrorCaptured')
      // ...
    })
  }
}

</script>

<style lang="scss">
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
