<template>
    <div class="nev">
        <div class="top">
            <button onclick="window.location.href='/home'" class="button_btn">Home</button>
            <button onclick="window.location.href='/login'" class="button_btn">นัดหมาย</button>

            <div class="search">
                <input  class="input_search" type="text" value="">
                <div class="search_icon">
                    <button class="myicon">
                        <!-- <img src="https://cdn2.iconfinder.com/data/icons/ios-7-icons/50/search-512.png"> -->
                    </button>          
                </div>
            </div>

            <button class="button_btn">แจ้งเตือน</button>
            <button class="button_btn">ชื่อ-สกุล</button>
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
$bg:#E597FA;
$pd10:10px;

button{
    // font-weight: bold;
    font-size: 18px;
}
.nev{
    background: $bg;
    width: 100%;
    padding: $pd10;
    position: fixed;
    top:0;
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
                border: none;
                .myicon{
                    height: 100%;
                    width: 100%;
                    border: none;
                    align-items: center;
                    background-size: 100% 100%;
                    background-image: url("https://cdn2.iconfinder.com/data/icons/ios-7-icons/50/search-512.png");
                }
            }
        }
    }
}

</style>