<template>
    <div class="layout">
        <div class="background">
            <div class="back_white">
                <div class="topic-head">
                    <label>Register</label> 
                </div>
                <div><Forminput/></div>
                <div class="btn-position">
                    <nuxt-link to="/login">
                        <button class="btn-register">Register</button>
                    </nuxt-link>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import Forminput from '@/components/Forminput_register'
export default {
    components:{
        Forminput

    }
    
}
</script>

<style lang="scss" scopeed>
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
            .topic-head{
                text-align: center;
                font-size: 20px;
            }
            .btn-position{
                text-align: center;
                margin-top: 20px;
                .btn-register{
                    padding-bottom: 10px;
                    padding-top: 10px;
                    padding-left: 40px;
                    padding-right: 40px;
                    background: #55CF1C;
                    color: white;
                    border: none;
                    border-radius: 10px;
                    font-weight: bold;
                    box-shadow: 3px 3px rgba(0, 0, 0, 0.4);
                    transition: 0.4s ease-out;
                    &:hover {
                    box-shadow: 6px 6px rgba(0, 0, 0, 0.6);
                    }
                    // &:active{
                    //     border: none;
                    // }               
                }
            }

            // .input_data{
            //     display: flex;
            // }
        }
    }
}  
</style>