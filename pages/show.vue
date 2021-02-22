<template>
    <div class="display">
        <Nevbar></Nevbar>
        <div class="top">
            <div style="display:flex">
                <div>หัวข้อโปรเจค</div>
                <div class="img_next"></div>
                <div style="margin-left:1rem">
                    <Label>Design</Label>
                </div>
            </div>
            <div>
                <button class="btn_top" onclick="window.location.href='/edit'">แก้ไขโปรเจค</button>
                <button class="btn_top" onclick="window.location.href='/add_user'">เพิ่มสมาชิก</button>
                <button class="btn_top">Github</button>
                <button class="btn_top" onclick="window.location.href='/progress_page'">เพิ่มความคืบหน้า</button>
            </div>
        </div>

        <div class="down">
            <div class="down_info">
                <div class="card_down_name">
                    <Label>ความคืบหน้า</Label>
                </div>
                
                <div class="list_card">
                    <Card/>
                    <Card/>
                    <Card/>
                    <Card/>
                    <Card/>
                    <Card/>
                    <Card/>
                    <Card/>
                    <!-- <Card/>
                    <Card/>
                    <Card/>
                    <Card/>
                    <Card/>
                    <Card/>
                    <Card/> -->
                </div>
            
            </div>
        </div>


    </div>    
</template>

<script>
import Nevbar from '@/components/nevbar'
import Card from '@/components/card_show'
export default {
    components:{
        Nevbar,Card
    },
    data(){
        return{
                imgCard: 'https://img.rawpixel.com/s3fs-private/rawpixel_images/website_content/v462-n-130-textureidea_1.jpg?w=800&dpr=1&fit=default&crop=default&q=65&vib=3&con=3&usm=15&bg=F4F4F3&ixlib=js-2.2.1&s=9465282a2b0a375f4f5b120d7bbad882',
                cardName: 'Monkey D. Luffy',
                cardDate: 'กัปตัน'

        }     
    },
    // methods: {
    //    setDataSearch(data){
    //        console.log(data)
    //        this.textSearchTitle = data
    //    }
    // },
    // computed:{
    //     filterSearch(){
    //         if(this.textSearchTitle === ''){
    //             return this.listCard
    //         }else{
    //             return this.listCard.filter((card,i) => {
    //                 return card.title.includes(this.textSearchTitle)
    //             })
    //         }   
    //     }
    // }
    
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Prompt:100,200,400,500,600,700&display=swap');

*{font-family: 'Prompt', sans-serif;}

.display{
    width: 100vw;
    height: 100vh;
    padding-top: 3rem;
    .top{
        // background: #7fff00;
        display: flex;
        padding: 1rem;
        justify-content: space-between;
        // padding-top: 1rem;
        // .btn_top{
        //     padding: 10px;
        //     font-size: 18px;
        //     border-radius: 10px;
        //     background: hsl(0, 12%, 91%);
        //     border: none;
        // }
        .img_next{
            padding: 7px;
            margin-left: 1rem;
            // border: 1px solid black;
            background-size: 100% 100%;
            background-image: url('https://www.flaticon.com/svg/vstatic/svg/626/626053.svg?token=exp=1613400504~hmac=3c832da7a4098f3f7058861400220693');
        }
    }
    .down{
        padding: 15px;
        // background: blueviolet;
        .down_info{
            // border: 1px solid black;
            border-radius: 5px;
            box-shadow: 5px 5px 10px 5px rgba(224,224,224,0.5);
            .card_down_name{
            background: #F2DDFF;
            padding: 5px;
            border-radius: 5px 5px 0 0;
            }
            .list_card{
            background: white;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 5px;
            border-radius: 0 0 5px 5px;
            }
        }


    }
}
</style>