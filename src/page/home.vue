<template>
    <div class="fillcontain home_page">
        <head-top></head-top>
        <section class="data_section">
            <header class="section_title">当日数据统计</header>
            <el-row :gutter="20">
                <el-col :span="8"><div class="data_list"><span class="data_num">1,621</span>浏览量</div></el-col>
                <el-col :span="8"><div class="data_list"><span class="data_num">13,087</span>API请求量</div></el-col>
                <el-col :span="8"><div class="data_list"><span class="data_num">143</span>新增用户</div></el-col>
            </el-row>
        </section>
    </div>
</template>
<script>
    import headTop from '../components/headTop'
    export default {
        components: {
            headTop
        }
    }
</script>

<style lang="less">
    @import '../style/mixin';
    .data_section{
        padding: 20px;
        .section_title{
            text-align: center;
            font-size: 30px;
            margin-bottom: 10px;
        }
        .data_list{
            text-align: center;
            font-size: 14px;
            .data_num{
                color: #333;
                font-size: 26px;
            }
        }
    }
</style>
