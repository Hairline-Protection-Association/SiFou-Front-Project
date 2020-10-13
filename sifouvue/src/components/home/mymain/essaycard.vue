<template>
    <div class="essaycardstyle">
        <div>   
            <div class="title">
                文章标题
            </div>
            <div style="display: flex; margin-top: 10px">
                <!-- 文章内容部分 -->
                <div class="excerpt">
                    内容节选:这个节日是守护者们满足甜食欲望，戴上不敬的面具来纪念失去之人回忆的时间。金字塔飞船于黑暗之中涌动着，
                    木卫二等待着你，暗影向你发出召唤。字数限制...
                </div>
                <img src="../../../assets/logo.png" >
            </div>
            <div style="display: flex">
                <!-- cardfooter -->
                <div style="displya: flex">
                    <!-- 点赞 -->
                    <Icon type="ios-thumbs-up-outline" />
                    x
                    <span>number</span>
                </div>
                <div style="margin-left: 10px">
                    <!-- 作者 -->
                    name
                </div>
                <div style="margin-left: 10px">
                    <!-- 日期  -->
                    - data
                </div>
            </div>
            

        </div>
      
    </div>
</template>
<script>
export default {
    name: 'essaycard',

}
</script>
<style lang="less" scoped>
    .essaycardstyle{
        .title{
            width: 635px;
            font-size: 18px;

        }
        .excerpt{
            width: 85%;
            height: 80px;
            font-size: 14px;
            color: #888888;
        }
        img{
            width: 60px;
            margin-left: 20px;
        }
    }
</style>