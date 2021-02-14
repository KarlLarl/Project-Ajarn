<template>
    <div class="main">
        <nevbar></nevbar>
        <div class="detail">
            <div class="create_top">
                <label class="top_name">สร้างหัวข้อ</label>
            </div>
            <!-- ข้อมูลการกรอก -->
            <div class="input_info">
                <div class="left">
                    หัวข้อโปรเจค :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>

            <div class="input_info">
                <div class="left">
                    อาจารย์ที่ปรึกษาโปรเจค :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>

            <div class="input_info">
                <div class="left">
                    วัน/เดือน/ปี :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>

            <div class="input_info">
                <div class="left">
                    Github/Gitlab :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>
        </div>

        <div class="btn">
            <div><button class="btn_size" style="background:#2957F8">บันทึก</button></div>
            <div><button class="btn_size" style="background:#FB5959">ยกเลิก</button></div>
        </div>

    </div>
</template>
<script>
import nevbar from '@/components/nevbar'
export default {
    components:{
        nevbar
    }
}
</script>
<style lang="scss" scoped>
.main{
    background: white;
    width: 100vw;
    height: 100vh;
    padding-top: 6rem;
    .detail{
        .create_top{
            // background: chartreuse;
            text-align: center;
            padding: 10px;
            padding-bottom: 3rem;
            .top_name{
                // font-weight: bold;
                font-size: 28px;
            }
        }
        .input_info{
            // background: red;
            display: flex;
            width: 100%;
            padding-bottom: 20px;
            .left{
                width: 50%;
                padding-left: 20rem;
                flex-direction: column;
                justify-content: center;
                display: flex;
            }
            .right{
                width: 50%;
                .input_right{
                    background: #F5EBEB;
                    border-radius: 7px;
                    border: 1px solid black;
                    padding: 10px;
                    width: 75%;
                }
            }
        }    
    }
    .btn{
        text-align: center;
        margin-top: 3rem;
        .btn_size{
            padding: 10px;
            border: 1px solid black;
            border-radius: 7px;
            width: 25%;
            margin-bottom: 10px;
            color: white;
            font-weight: bold;
            font-size: 18px;
        }
    }
}

</style>