<template>
    <div class="main">
        <nevbar></nevbar>
        <forminput></forminput>

        <div class="btn">
            <div><button class="btn_size" style="background:#2957F8">ยืนยัน</button></div>
            <div><button class="btn_size" style="background:#FB5959">ยกเลิก</button></div>
        </div>

    </div>
</template>
<script>
import nevbar from '@/components/nevbar'
import forminput from '@/components/Forminput'
export default {
    components:{
        nevbar,forminput
    }
}
</script>
<style lang="scss" scoped>
.main{
    background: white;
    width: 100vw;
    height: 100vh;
    padding-top: 6rem;
    .btn{
        text-align: center;
        margin-top: 3rem;
        .btn_size{
            padding: 10px;
            border: none;
            border-radius: 7px;
            width: 25%;
            margin-bottom: 1rem;
            color: white;
            font-weight: bold;
            font-size: 18px;
            box-shadow: 3px 3px rgba(0, 0, 0, 0.4);
            transition: 0.4s ease-out;
            &:hover {
            box-shadow: 6px 6px rgba(0, 0, 0, 0.6);
            }
        }
    }
}
// @media screen and (max-width: 899px) /*จอเล็ก*/{
// .left{
//   width: 50%;
//   padding-left: 10rem;
//   flex-direction: column;
//   justify-content: center;
//   display: flex;
//     }
//   }
</style>