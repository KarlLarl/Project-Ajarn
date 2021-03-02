<template>
    <div class="main">
        <nevbar></nevbar>
        <div class="top">
            <div style="font-size: 1rem; margin-left: 1rem;">หัวข้อทั้งหมด</div>
            <button class="btn-top" onclick="window.location.href='/create_topic'">สร้างหัวข้อ</button>
        </div>

        <div class="down">
            <Card v-for=" (card,index) in listCard" :key="index"
            :cardName="card.cardName"
            :cardDate="card.cardDate" />    
        </div>
        <!-- TEST -->
    </div>   
</template>
<script>
import nevbar from '@/components/nevbar'
import Card from '@/components/card_home'
export default {
    components:{
        nevbar,Card
    },
    data(){
        return{
            listCard:[
                {
                    cardName:'Card_1',
                    cardDate:'1/1/1'
                },
                {
                    cardName:'Card_2',
                    cardDate:'2/2/2'
                },
                {
                    cardName:'Card_3',
                    cardDate:'3/3/3'
                },
                {
                    cardName:'Card_4',
                    cardDate:'4/4/4'
                },
                {
                    cardName:'Card_5',
                    cardDate:'5/5/5'
                },
                {
                    cardName:'Card_6',
                    cardDate:'6/6/6'
                },
                {
                    cardName:'Card_7',
                    cardDate:'7/7/7'
                },
                {
                    cardName:'Card_8',
                    cardDate:'8/8/8'
                },
            ]
        }
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
            font-size: 1rem;
            // font-weight: bold;
            border-radius: 10px;
            background: #EAE4E4;
            border: none;
            box-shadow: 3px 3px rgba(0, 0, 0, 0.4);
            transition: 0.4s ease-out;
            &:hover {
            box-shadow: 6px 6px rgba(0, 0, 0, 0.6);
            }
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