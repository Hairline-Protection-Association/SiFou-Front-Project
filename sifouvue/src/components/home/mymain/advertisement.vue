<template>
    <div class="advertisementstyle">
        <div class="textad">
            <!-- 文字广告 -->
            <a href="" class="textadinner">这里是文字广告zhe li shi wen zi guang gao 这里理应包一层之后再说</a>
        </div>
            <!-- 图片广告 -->
            <img style="margin-top: 20px" src="../../../assets/images/guanggao1.png" alt="">
            <img style="margin-top: 20px" src="../../../assets/images/guanggao3.png" alt="">
            <img style="margin-top: 20px" src="../../../assets/images/guanggao2.png" alt="">
            <div>
                <!-- 活动推荐 -->
                <div style="display: flex;margin-top:20px;">
                    <span style="font-size: 18px">活动推荐</span>
                    <a style="color: lightgreen; margin-left: 140px;font-size:18px" href="">更多</a>
                </div>
            <br>
                <img src="../../../assets/images/huodong.png" alt="">
            </div>
            <img style="margin-top: 20px" src="../../../assets/images/guanggao4.png" alt="">
            
    </div>
</template>

<script>
export default {
    name: 'advertisement'
}
</script>
<style lang="less" scoped>
    .advertisementstyle{
        width: 250px;
        margin-left: 20px;
        .textad{
            background: rgb(252, 248, 227);
            border-radius: 5px;
            height: 70px;
            border: solid 0.5px brown;
            .textadinner{
                color: saddlebrown;
                font-size: 12px;
                text-align: center;
                padding-left: 20px;
            }
        }
    }
</style>