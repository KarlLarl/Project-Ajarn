<template>
    <div class="back">
        <div class="card">
            <!-- หัวข้อด้านบน -->
            <div class="card_top">
                <div class="txt_top">
                    <div><h4>หัวข้อโปรเจค</h4></div>
                    <div><h6>วันเวลา</h6></div>
                </div>
                <div><button class="btn-card-top"></button></div>
            </div>
            <!-- เนื้อหา Topic คืบหน้า -->
            <div class="all_small">
                <div class="small_topic_card" style="margin-top:10px">
                    <div class="topic_small">
                        Requirments
                    </div>
                    <div style="margin-top:20px">
                        วันนัดหมาย
                    </div>
                </div>

                <div class="small_topic_card" style="margin-top:10px">
                    <div class="topic_small">
                        Login
                    </div>
                    <div style="margin-top:20px">
                        วันนัดหมาย
                    </div>
                </div>
                

                <div class="small_topic_card" style="margin-top:10px">
                    <div class="topic_small">
                        Common
                    </div>
                    <div style="margin-top:20px">
                        วันนัดหมาย
                    </div>
                </div>

                <div class="small_topic_card" style="margin-top:10px">
                    <div class="topic_small">
                        Finish
                    </div>
                    <div style="margin-top:20px">
                        วันนัดหมาย
                    </div>
                </div>

                
            </div>
            <!-- btn ด้านล่าง -->
            <div class="card_down">
                <button>add topic card</button>
                <button>GitHub</button>
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
<style lang="scss" scoped>
/* width */
::-webkit-scrollbar {
  width: 5px;
  height: 5px;
}

// /* Track */
// ::-webkit-scrollbar-track {
//   background: #f1f1f1; 
// }
 
// /* Handle */
// ::-webkit-scrollbar-thumb {
//   background: #888; 
// }

// /* Handle on hover */
// ::-webkit-scrollbar-thumb:hover {
//   background: #555; 
// }
h6{
    margin-left: 5px;
}
.back{
    padding: 10px;
    .card{
        background: #F2DDFF;
        padding: 10px;
        width: fit-content;
        border-radius: 10px;
        height: 300px;
        .card_top{
            display: flex;
            justify-content: space-between;
            .txt_top{
                display: flex;
                align-items: baseline;
            }
            .btn-card-top{
                height: 100%;
                background-image: url("https://image.flaticon.com/icons/png/512/84/84380.png");
                background-size: cover;
                border: none;
                width: 21px;
            }
        }
        .all_small{
            margin-top: 10px;
            height: 220px;
            overflow: auto;
            
            .small_topic_card{
            background: white;
            width: 230px;
            border-radius: 10px;
            padding: 5px;
            font-weight: bold;
            } 
        }

        .card_down{
            display: flex;
            justify-content: space-between;
            align-items: baseline;
            margin-top: 10px;
        }
    }
}
</style>