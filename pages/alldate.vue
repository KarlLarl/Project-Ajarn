<template>
    <div class="main">
        <nev/>
        <div class="showdata">
            <div class="top_img">
                <div class="shadow">
                    <div class="top_img_name">
                        <label for="">TEST</label> 
                    </div>
                    <div class="list_img">
                        <label for="">
                            <img :src="img" >
                        </label>
                    </div>
                </div>
            </div>
            <div class="top_file">

            </div>
            <div class="top_comment">
                
            </div>
        </div>
    </div>
</template>

<script>
import nev from '@/components/nevbar'
export default {
    components:{
        nev
    },
    data(){
        return {
        img:'https://www.flaticon.com/svg/vstatic/svg/622/622669.svg?token=exp=1614490330~hmac=30c7f7f62c7e3c90d83946dd444e6d10'
        }
    }
}
</script>

<style lang="scss">
.shadow{
box-shadow: 5px 5px 10px 5px rgba(224,224,224,0.5);
transition: 0.4s ease-out;

}
.main{
    background: white;
    width: 100vw;
    height: 100vh;
    // margin-bottom: 3rem;
    .showdata{
        // margin-top: 1rem;
        // padding-top: 5rem;
        // background:violet;
        padding: 5rem 5rem 0 5rem; //บน ซ้าย ขวา กลาง
        .top_img{
            // background: rgba(0,0,0,0.5);
            // background:violet;
            // width: fit-content;
            background-color: transparent;
            padding: 12px;
            .top_img_name{
                background: violet;
                // width: 100%;
                padding: 0.5rem;
                border-radius: 12px 12px 0 0;
            }
            .list_img{
                // background: rgb(211, 211, 192);
                padding: 1rem;
                border-radius: 0 0 12px 12px;
            }
        }

    }
}
</style>