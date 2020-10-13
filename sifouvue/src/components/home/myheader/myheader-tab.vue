<template>
    <div class="mytab">
       <Button class="everytabbtn" type="text" ghost>首页</Button>
       <Button class="everytabbtn" type="text" ghost>问答</Button>
       <Button class="everytabbtn" type="text" ghost>专栏</Button>
       <Button class="everytabbtn" type="text" ghost>资讯</Button>
       <Button class="everytabbtn" type="text" ghost>课程</Button>
       <Button class="everytabbtn" type="text" ghost>活动</Button>
        <Dropdown placement="bottom-start" style="transform: translate(25px,1px);">
        <a href="javascript:void(0)" style=" color:  #999999;">
            发现
            <Icon type="ios-arrow-down"></Icon>
        </a>
        <DropdownMenu slot="list" style="text-align: left">
            <DropdownItem>圈子</DropdownItem>
            <DropdownItem>标签</DropdownItem>
            <DropdownItem>酷工作</DropdownItem>
            <DropdownItem>排行榜</DropdownItem>
            <DropdownItem>徽章</DropdownItem>
            <DropdownItem>笔记</DropdownItem>
            <DropdownItem>开发手册</DropdownItem>
            <DropdownItem>广告投放</DropdownItem>
        </DropdownMenu>
    </Dropdown>
    </div>
</template>

<style lang="less" scoped>
    .mytab{
        width: 440px; 
        .everytabbtn{
            width: 50px;
            height: 30px;
            text-align: center;
            color: #999999;

        }
    }

</style>

<script>
export default {
    name: 'myheadertab'
}
</script>