<template>
    <div class="nev">
        <div class="top">
            <button onclick="window.location.href='/home'" class="button_btn">Home</button>
            <button onclick="window.location.href='/appointment'" class="button_btn">นัดหมาย</button>

            <div class="search">
                <input  class="input_search" type="text" value="">
                <div class="search_icon">
                    <a onclick="window.location.href='/create_topic'">
                        <div class="myicon"></div>
                    </a>        
                </div>
            </div>

            <button class="button_btn">แจ้งเตือน</button>
            <button class="button_btn" onclick="window.location.href='/login'">ชื่อ-สกุล</button>
        </div>
    </div>
</template>
<script>
export default {
    // data(){
    //     return{
    //         icon_url:'https://cdn2.iconfinder.com/data/icons/ios-7-icons/50/search-512.png'
    //     }
    // }
    
}
</script>
<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Prompt:100,200,400,500,600,700&display=swap');

*{font-family: 'Prompt', sans-serif;}

$bg:#E597FA;
$pd10:10px;

button{
    // font-weight: bold;
    font-size: 1rem;
}
.nev{
    background: $bg;
    width: 100%;
    padding: $pd10;
    position: fixed;
    top:0;
    box-shadow: 5px 5px 5px 5px rgba(224,224,224,0.5); 
    // box-shadow: 6px 6px rgba(0, 0, 0, 0.6);
    .top{
        background: $bg;
        padding-left: $pd10;
        padding-right: $pd10;
        display: flex;
        justify-content: space-between;
        .button_btn{
            background: $bg;
            border: none;
            outline: none;
        }
        .search{
            background: white;
            display: flex;
            width: 30%;
            height: 30px;
            .input_search{
                width: 90%;
                border: none;
                padding: 10px;
            }
            .search_icon{
                width: 10%;
                padding: 5px;
                // border: none;
                .myicon{
                    height: 100%;
                    // width: 100%;
                    // border: 1px solid black;
                    // align-items: center;
                    background-size: 100% 100%;
                    background-image: url("https://cdn2.iconfinder.com/data/icons/ios-7-icons/50/search-512.png");
                }
            }
        }
    }
}
@media screen and (max-width: 700px) {
    button{font-size: 12px;}
    .nev .top .search .input_search{
                width: 70%;
            }
    .nev .top .search .search_icon{
                width: 30%;
    }
}
</style>