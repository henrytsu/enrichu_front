<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/images/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    
    <el-row  class="container">
      <el-col :span="24">
        <TopMenu msg="Welcome to Your Vue.js App" />
      </el-col>
      <el-col :span="24">
        <LeftNav />
        <!-- <section class="content-container"> -->
          <div class="grid-content">
            ContentSection
            <transition name="fade" mode="out-in">
              
            </transition>
          </div>
        <!-- </section> -->
      </el-col>
    </el-row>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import TopMenu from "./components/TopMenu.vue";
import LeftNav from "@/components/LeftNav";

export default {
  name: "App",
  components: {
    TopMenu,
    LeftNav
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
