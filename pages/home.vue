<template>
    <div class="main">
        <nevbar></nevbar>
        <div class="top">
            <div>หัวข้อทั้งหมด</div>
            <button class="btn-top" onclick="window.location.href='/create_topic'">สร้างหัวข้อ</button>
        </div>
        <div class="down">
            <!-- <card></card>
            <card></card>
            <card></card>
            <card></card>
            <card></card>
            <card></card> -->
            <Card/>
            <Card/>
            <Card/>
            <Card/>
            <Card/>
        </div>
    </div>   
</template>
<script>
import nevbar from '@/components/nevbar'
import card from '@/components/card'
import Card from '@/components/card_home'
export default {
    components:{
        nevbar,card,Card
    }

}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Prompt:100,200,400,500,600,700&display=swap');

*{font-family: 'Prompt', sans-serif;}

.main{
    background: white;
    width: 100vw;
    height: 100vh;
    padding-top: 3rem;
    .top{
        display: flex;
        justify-content: space-between;
        // font-weight: bold;
        font-size: 18px;
        align-items: center;
        padding-bottom: 15px;
        padding-top: 15px;
        padding-left: 10px;
        padding-right: 10px;
        // position: fixed;
        // width: 100%;
        .btn-top{
            padding: 10px;
            font-size: 18px;
            // font-weight: bold;
            border-radius: 10px;
            background: #EAE4E4;
            border: none;
            // background-image: url("https://upload.wikimedia.org/wikipedia/commons/thumb/6/64/Edit_icon_%28the_Noun_Project_30184%29.svg/1024px-Edit_icon_%28the_Noun_Project_30184%29.svg.png");
        }
    }
    .down{
        display: flex;
        flex-flow: wrap;
        // width: 100%;
        justify-content: center;
    }
}
</style>