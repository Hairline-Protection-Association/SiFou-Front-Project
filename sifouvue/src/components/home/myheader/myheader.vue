<template>
    <div class="headercomponent">
        <img src="../../../assets/images/sifou-logo.png">
        <Myheadertab style="text-align: center; margin: 15px; transform: translate(390px,0)"></Myheadertab>
        <Myheadersearch style="margin: 15px; transform: translate(360px,0)" ></Myheadersearch>
        <div class="doublebutton">
            <Button type="success" ghost>立即登录</Button>
            <Button type="success" style="transform: translate(10px,0); width: 50%;">免费注册</Button>
        </div>
    </div>
</template>

<style lang="less" scoped>
    .headercomponent{
        height: 60px;
        width: 100%;
        display: flex;
        background-color:rgb(250, 250, 250);
        box-shadow: 1px 1px 1px rgb(200, 200, 200);
        img{
            margin: 5px;
            transform: translate(440px,0);
        }
        .doublebutton{
            display: flex;
            margin: 15px;
            transform: translate(420px,0);
        }
    }
</style>

<script>
import Myheadertab from './myheader-tab'
import Myheadersearch from './myheader-search'
export default {
    name: 'myheader',
    components: {
        Myheadertab,
        Myheadersearch,
    }
    
}
</script>