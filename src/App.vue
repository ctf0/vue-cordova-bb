<template>
  <div id="app">
    <div>
      <img src="static/logo.png">
      <router-view/>
    </div>
  </div>
</template>

<style src="@/assets/main.scss" lang="scss"></style>

<script>
export default {
  name: 'App',
  created() {
      document.addEventListener('deviceready', this.onDeviceReady)
  },
  methods: {
    onDeviceReady() {
        this.onResume()
        document.addEventListener('resume', this.onResume)
        document.addEventListener('pause', this.onPause)
        document.addEventListener('online', this.onOnline)
        document.addEventListener('offline', this.onOffline)
    },
    onResume() {
    },
    onPause() {
    },
    onOnline() {
    },
    onOffline() {
    }
  }
}
</script>
