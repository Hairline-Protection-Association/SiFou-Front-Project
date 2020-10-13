<template>
    <div class= "essayliststyle">
        <!-- 选择文章种类的标题 -->
        <div style="font-size: 18px;transform: translate(0,10px);">为您推荐</div>
        <Divider/>
        <Essaycard></Essaycard>
    </div>
</template>
    
<script>
import Essaycard from './essaycard'
export default {
    name: 'essaylist',
    components: {
        Essaycard
    }
}
</script>
<style lang="less" scoped>
    .essayliststyle{
        width: 635px;
    }
</style>