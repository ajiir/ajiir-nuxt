<template>
<el-container>
  <el-header style="text-align: right; font-size: 12px">
    <el-dropdown>
      <i class="el-icon-setting" style="margin-right: 15px"></i>
      <el-dropdown-menu slot="dropdown">
        <el-dropdown-item>View</el-dropdown-item>
        <el-dropdown-item>Add</el-dropdown-item>
        <el-dropdown-item>Delete</el-dropdown-item>
      </el-dropdown-menu>
    </el-dropdown>
    <span>ajiir</span>
  </el-header>
  <el-main>
    <el-table :data="tableData">
      <el-table-column prop="date" label="Date" width="140">
      </el-table-column>
      <el-table-column prop="name" label="Name" width="120">
      </el-table-column>
      <el-table-column prop="address" label="Address">
      </el-table-column>
    </el-table>
  </el-main>
  </el-container>
</template>

<script>
export default {
name: 'Header',
  props: {
    tableData: {
    type: Array,
    default: () => null
  }
}
}
</script>
<style>
  .el-header {
    background-color: #B3C0D1;
    color: #333;
    line-height: 60px;
  }
</style>