<template>
    <div class="layout">
        <div class="background">
            <div class="back_white">
                <div class="input_data">
                    <div style="text-align: center;"><h3>ระบบที่ปรึกษาโปรเจคกับอาจารย์</h3></div>
                    <div class="txt_input"><Forminput/></div>
                    <div class="btn-flex">
                        <div class="fix-size">
                            <div><button onclick="window.location.href='/home'" class="btn-login" >Login</button></div>
                            <div><button onclick="window.location.href='/home'" class="btn-facebook">Facebook</button></div>
                            <!-- <div><button class="btn-facebook">
                                <div class="img-facebook"></div>
                                Facebook
                                </button>
                            </div>                        -->    
                        </div>
                    </div>
                    <div class="flex-row">
                        <div style="font-size:14px;"> Forgot : </div>
                        <nuxt-link to=""><div class="user-pass" style="font-size:14px;">Username / Password ?</div></nuxt-link>
                    </div>

                    <div><nuxt-link to="/register"><div class="create">Create your Account</div></nuxt-link></div>

                </div>
            </div>

        </div>
    </div>
</template>
<script>
import Forminput from '@/components/Forminput'
export default {
    components:{
        Forminput

    }
}
</script>
<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Prompt:100,200,400,500,600,700&display=swap');

*{font-family: 'Prompt', sans-serif;}
.layout{
    width: 100vw;
    height: 100vh;
    .background{
        height: 100%;
        background: linear-gradient(243.75deg, #FC84F0 0.82%, #6A76E3 99.92%, rgba(255, 187, 187, 0) 100%);
        display: flex;
        justify-content: center;
        align-items: center;
        .back_white{
            background:  white;  
            padding-right: 50px;
            padding-left: 50px;
            padding-top: 40px;
            padding-bottom: 40px;
            border-radius: 5px;
            align-items: center;
            width: 60%;
            .input_data{
                display: flex;
                flex-direction: column;

                .txt_input{
                    display: flex;
                    flex-direction: column;
                    padding-top: 10px;
                    padding-bottom: 10px;
                }
                .btn-flex{
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    margin-bottom: 10px;
                    .fix-size{
                        width: 40%;
                    }
                    .btn-login{
                    padding: 10px;
                    background: #325EFB;
                    border-radius: 10px;
                    width: 100%;
                    border:none;
                    color: white;
                    font-weight: bold;
                    font-size: 15px;
                    margin-bottom: 10px;
                    }
                    .btn-facebook{
                    margin-bottom: 10px;
                    width: 100%;
                    background-color: #4D6EE1;
                    border: none;
                    color: white;
                    font-weight: bold;
                    font-size: 15px;
                    border-radius: 10px;
                    padding:10px;
                    text-align: center;
                        // .img-facebook{
                        //     width: 18px;
                        //     height: 18px;
                        //     background-image: url('~@/assets/facebook.png');
                        //     background-repeat: round;
                        //     margin-right: 30px;
                        // }
                    }
                }
            .flex-row{
                display: flex;
                flex-direction: row;
                justify-content: center;
                .user-pass{
                color: red;
                margin-left: 5px;
                    }
                }
            .create{
                margin-top: 10px;
                color: #325EFB;
                text-align: center;
            }
            }
        }
    }
}
</style>