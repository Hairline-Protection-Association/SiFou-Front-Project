<template>
    <div class="mymainstyle">
       <Essaykind></Essaykind>
       <div>
            <!-- 轮播图 -->
            <Carousel autoplay loop style="width:635px; height: 150px;">
                <CarouselItem >
                    <div >
                        <img style="width:635px; height: 150px;  border-radius: 5px;" src="https://image-static.segmentfault.com/129/968/1299681570-5f7815bbf07c4">
                    </div>
                </CarouselItem>
                <CarouselItem>
                    <div>
                        <img style="width:635px; height: 150px; border-radius: 5px;" src="https://image-static.segmentfault.com/109/185/1091855226-5f69bdd55c3a7">
                    </div>
                </CarouselItem>
                <CarouselItem>
                    <div>
                        <img style="width:635px; height: 150px; border-radius: 5px;" src="https://image-static.segmentfault.com/146/815/1468153747-5f5c2157ce9a0">
                    </div>
                </CarouselItem>
            </Carousel>
            <!-- 文章列表 -->
            <Essaylist></Essaylist>
       </div>
       <Advertisement></Advertisement>
    </div>
</template>

<style lang="less" scoped>
    .mymainstyle{
        height: 100%;
        width: 52%;
        margin-left: 23%;
        margin-top: 30px;
        display: flex;
    }
</style>

<script>
import Essaykind from './essaykind'
import Essaylist from './essaylist'
import Advertisement from './advertisement'
export default {
    name: 'mymain',
    components: {
        Essaykind,
        Essaylist,
        Advertisement
    }
    
}
</script>