<template>
  <el-row>
    <el-col :span="24" class="topbar-wrap">
      <div class="topbar-logo topbar-btn">
        <a href="/"><img src="../assets/images/logo.png"></a>
      </div>
      <div class="topbar-logos" v-show="!collapsed">
        <a href="/"  style="color: #AfAfAf;font-size:22px;font-bold:true">EnrichU</a>
      </div>
      <div class="topbar-title">
        <el-row>
          <el-col :span="24">
            <el-menu
              class="el-menu-demo"
              mode="horizontal"
              @select="handleSelect"
              :router="true"
            >
              <el-menu-item index="/">工作台</el-menu-item>
              <el-menu-item index="/enterpriseManager">企业管理</el-menu-item>
              <el-menu-item index="/orderManager">订单管理</el-menu-item>
              <el-menu-item index="/systemManager">系统管理</el-menu-item>
            </el-menu>
          </el-col>
        </el-row>
      </div>
    </el-col>
  </el-row>
</template>

<script>
export default {
  name: "TopMenu",
  props: {
    msg: String
  }
};
</script>