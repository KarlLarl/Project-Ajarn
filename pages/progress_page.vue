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
        // text-align: center;
        margin-top: 3rem;
        display: flex;
        justify-content: space-evenly;
        .btn_size{
            padding: 10px;
            padding-left: 5rem;
            padding-right: 5rem;
            border: 1px solid black;
            border-radius: 7px;
            margin-bottom: 10px;
            color: white;
            font-weight: bold;
            font-size: 18px;
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