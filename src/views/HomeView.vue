<template>
    <div>
        <!-- 搜索框   -->
        <div style="margin-bottom: 20px; margin-top: 5px; margin-left: 3px">
            <el-input style="width: 240px" placeholder="请输入名称"></el-input>
            <el-input style="width: 240px; margin-left: 8px" placeholder="请输入联系方式"></el-input>
            <el-button style="margin-left: 5px" type="primary"><i class="el-icon-search"></i>搜索</el-button>

        </div>

        <el-table :data="tableData" stripe>
            <el-table-column prop="name" label="名称"></el-table-column>
            <el-table-column prop="age" label="年龄"></el-table-column>
            <el-table-column prop="address" label="地址"></el-table-column>
            <el-table-column prop="phone" label="联系方式"></el-table-column>
            <el-table-column prop="sex" label="性别"></el-table-column>
        </el-table>


        <!-- 分页 -->
        <div style="margin-top: 20px">
            <el-pagination
                background
                :page-size="5"
                layout="prev, pager, next"
                :total="tableData.length">
            </el-pagination>
        </div>

  </div>
</template>

<script>
export default {
    name: 'HomeView',
    data() {
        return {
            tableData: [
                { name: '张三', age: 20, address: '浙江省', phone: '15905890000', sex: '男'},
                { name: '张三', age: 20, address: '浙江省', phone: '15905890000', sex: '男'},
                { name: '张三', age: 20, address: '浙江省', phone: '15905890000', sex: '男'},
                { name: '张三', age: 20, address: '浙江省', phone: '15905890000', sex: '男'},
                { name: '张三', age: 20, address: '浙江省', phone: '15905890000', sex: '男'},
                { name: '张三', age: 20, address: '浙江省', phone: '15905890000', sex: '男'},
                { name: '张三', age: 20, address: '浙江省', phone: '15905890000', sex: '男'},
                { name: '张三', age: 20, address: '浙江省', phone: '15905890000', sex: '男'},
                { name: '张三', age: 20, address: '浙江省', phone: '15905890000', sex: '男'},
                { name: '张三', age: 20, address: '浙江省', phone: '15905890000', sex: '男'},
                { name: '张三', age: 20, address: '浙江省', phone: '15905890000', sex: '男'}
            ]



        }


    }



}
</script>
