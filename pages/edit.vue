<template>
<div class="background">
    <nevbar/>
    <form class="edit">
        <div class="top_head">
            <label>แก้ไขโปรเจค</label>
        </div>
        <div class="edit_detail">
            <div class="input_detail">
                <label>ชื่อโปรเจค</label>
                <input type="text">
            </div>
        </div>

    </form>


</div>
    
</template>
<script>

import nevbar from '@/components/nevbar'
export default {
    data(){
        return
    },
    components:{
        nevbar
    }    
}
</script>


<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Prompt:100,200,400,500,600,700&display=swap');

*{font-family: 'Prompt', sans-serif;}

.background{
    background: white;
    width: 100vw;
    height: 100vh;
    padding-top: 3rem;
    .edit{
        padding: 3rem;
        .top_head{
            font-size:2rem;
        }
        .edit_detail{
            margin-top: 3rem;
        }

    }
}
</style>