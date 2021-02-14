<template>
<div class="main">
    <!-- <nevbar></nevbar> -->
    <!-- <div class="top">
        <label>หัวข้อทั้งหมด</label>
        <button class="btn-top">สร้างหัวข้อ</button>
    </div> -->
    <div class="Card">
        <card></card>
        <card></card>
        <card></card>
        <card></card>
        <card></card>
    </div>

</div>
    
</template>
<script>
import nevbar from '@/components/nevbar'
import card from '@/components/card'
export default {
    components:{
        nevbar,card
    }
}
</script>
<style lang="scss" scoped>
.main{
    background: white;
    width: 100vw;
    height: 100vh;
    .top{
        background: red;
        margin-top: 3rem;
        // display: flex;
        // justify-content: space-between;
        // padding-left: 10px;
        // padding-right: 10px;
    }
}

</style>