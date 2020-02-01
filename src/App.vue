<template>
  <div id="app">
    <div class="container-fluid">
      <div class="scene">
        <div class="row justify-content-center align-content-end h-100">
            <div class="col-md-6 ">
                <div class="site-box">
                </div>
            </div>
        </div>
      <truck/>
      <helicopter/>
      <crane/>
      </div>
    </div>
  </div>
</template>

<script>
import Crane from './components/Crane.vue'
import Helicopter from './components/Helicopter.vue'
import Truck from './components/Truck.vue'

export default {
  name: 'app',
  components: {
    Crane,
    Helicopter,
    Truck
  }
}
</script>
<style lang="scss">
@import "./assets/wheel";

.container-fluid {
  padding: 0 !important;
}
.scene{
  height: 100vh;
  overflow: hidden;
  position:relative;
}

.site-box{
  width:646px;
  height:657px; 
  background: #000000;
}
</style>
