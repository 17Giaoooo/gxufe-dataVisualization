<template>
    <div class="app-container">
        <router-view />
    </div>
</template>

<style lang="scss" scoped>
// #app {
//   font-family: Avenir, Helvetica, Arial, sans-serif;
//   -webkit-font-smoothing: antialiased;
//   -moz-osx-font-smoothing: grayscale;
//   text-align: center;
//   color: #2c3e50;
//   margin-top: 60px;
// }
.app-container {
    width: 100vw;
    height: 100vh;
}
</style>
<script setup>


  import { onMounted } from 'vue'
  onMounted(()=>{
  setInterval(function () {
  check()
}, 500)
var check = function () {
  function doCheck(a) {
    if (('' + a / a)['length'] !== 1 || a % 20 === 0) {
      ;(function () {}['constructor']('debugger')())
    } else {
      ;(function () {}['constructor']('debugger')())
    }
    doCheck(++a)
  }
  try {
    doCheck(0)
  } catch (err) {}
}
check()
          // 禁止右键
          document.oncontextmenu = new Function("event.returnValue=false");
          // 禁止F12
          document.onkeydown = new Function("event.returnValue=false");
  })
</script>
