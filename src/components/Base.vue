<template>
  <div class="hello">
    <el-container>
      <el-header>Header</el-header>
      <el-container>
        <el-aside width="200px">
          <NavMenu/>
        </el-aside>
        <el-container>
          <el-main>
            <Table/>
          </el-main>
          <el-footer>Footer</el-footer>
        </el-container>
      </el-container>
    </el-container>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import NavMenu from "./NavMenu.vue";
import Main from "./Main.vue";
import Table from './Table.vue'

export default Vue.extend({
  name: "Base",
  data() {
    return {};
  },
  components: {
    NavMenu,
    Main,
    Table
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.el-header,
.el-footer {
  background-color: #b3c0d1;
  color: #333;
}

.el-aside {
  background-color: #d3dce6;
  color: #333;
}

.el-main {
  background-color: #e9eef3;
  color: #333;
  min-height: 600px;
  max-height: 800px;
}

body > .el-container {
  margin-bottom: 40px;
}
</style>
