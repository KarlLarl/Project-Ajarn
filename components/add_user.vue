<template>
    <div class="main" id="add_from">
        <div class="pop_user">
            <div class="header_pop">
                <label>เพิ่มสมาชิกเข้าโปรเจค</label>
            </div>
            <div class="detail_pop">
                <label>กรอก อีเมล ของผู้ใช้งานที่จะเพิ่มเข้าในโปรเจค</label>
            </div>
            <div class="input_email">
                <input class="input_sty" placeholder="คลิกเพื่อกรอกอีเมล" type="text">
                <button class="btn_sty">เพิ่ม</button>
            </div>

            <div class="close">
                <button class="btn_close" onclick="window.location.href='/show'">ปิด</button>
            </div>

        </div>
        
    </div>
</template>
<script>
export default {
    data(){
        return
    }
}
</script>
<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Prompt:100,200,400,500,600,700&display=swap');

*{font-family: 'Prompt', sans-serif;}
.main{
    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    .pop_user{
        background: white;
        width: 50%;
        height: fit-content;
        padding: 2rem;
        .detail_pop{
            margin-top: 1rem;
        }
        .close{
            margin-top: 12rem;
            display: flex;
            justify-content: flex-end;
            .btn_close{
            background: #e6e6e6;
            border: outset;
            color: #908787;
        }
        }

        .input_email{
            width: 100%;
            display: flex;
            margin-top: 1rem;
            .btn_sty{
                background: #e6e6e6;
                width: 20%;
                margin-left: 1rem;
                border: outset;
                color: #908787;
                // box-shadow: 5px 5px 5px 5px rgba(224,224,224,0.5); 
            }
            .input_sty{
                background: #e6e6e6;
                border: none;
                width: 80%;
                padding: 5px;
            }
        }
    }

}
</style>