<template>
    <div>
        <el-row>
            <el-col :span='7' class="post_list" id="order_list">
                111
            </el-col>
            <el-col :span='15'>
                222222222
            </el-col>

        </el-row>

    </div>
</template>

<script>
export default {
    name: 'Pos',
    data() {
        return {
            tableData: [{

                goodsName: '可口可乐',
                price: 8,
                count: 1
            }, {

                goodsName: '香辣鸡腿堡',
                price: 15,
                count: 1
            }, {

                goodsName: '爱心薯条',
                price: 8,
                count: 1
            }, {

                goodsName: '甜筒',
                price: 8,
                count: 1
            }]
        }
    },
    mounted: function() {
        var orderHeight = document.body.clientHeight;
        document.getElementById('order_list').style.height = orderHeight + "px";

    }
}
</script>
// #F9FAFC
<style scoped>
.post_list {
    background-color: #F9FAFC;
    border-right: #C0CCDA;
}
.div-btn {
    margin-top: 10px;
}
.title{
    height: 20px;
    border-bottom: 1px solid #d3dce6;
    background-color: #f9fafc;
    padding: 10px;
}
.often-goods-list ul li{
    list-style: none;
    float: left;
    border: 1px solid #e5e9f2;
    padding: 10px;
    margin: 5px;
    background-color: #fff;
}
.o-price{
    color: #58b7ff;
}
</style>
