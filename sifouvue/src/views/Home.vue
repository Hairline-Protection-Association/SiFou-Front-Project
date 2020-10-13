<template>
    <div>
        <Myheader></Myheader>
        <Mymain></Mymain>
    </div>
</template>

<script>
import Myheader from '../components/home/myheader/myheader'
import Mymain from '../components/home/mymain/mymain'
export default {
    name: 'Home',
    components: {
    Myheader,
    Mymain
    }
}
</script>

<style lang="less" scoped>
</style>