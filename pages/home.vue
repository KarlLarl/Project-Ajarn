<template>
    <div class="main">
        <nevbar></nevbar>
        <div class="top">
            <div>หัวข้อทั้งหมด</div>
            <button class="btn-top">สร้างหัวข้อ</button>
        </div>
        <div class="down">
            <card></card>
            <card></card>
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
    width: fit-content;
    height: 100vh;
    .top{
        display: flex;
        justify-content: space-between;
        font-weight: bold;
        font-size: 18px;
        align-items: center;
        padding-bottom: 15px;
        padding-top: 15px;
        padding-left: 10px;
        padding-right: 10px;
        .btn-top{
            padding: 10px;
            font-size: 18px;
            font-weight: bold;
            border-radius: 10px;
            background: #EAE4E4;
            border: none;
            // background-image: url("https://upload.wikimedia.org/wikipedia/commons/thumb/6/64/Edit_icon_%28the_Noun_Project_30184%29.svg/1024px-Edit_icon_%28the_Noun_Project_30184%29.svg.png");
        }
    }
    .down{
        display: flex;
        flex-flow: wrap;
        width: 100%;
    }
}
</style>