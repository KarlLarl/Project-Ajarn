<template>
    <div class="main">
        <nev/>
        <div class="showdata">
            <div class="top_img">

            </div>
            <div class="top_file">

            </div>
            <div class="top_comment">
                <label >TEST</label>
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
        return
    }
}
</script>

<style lang="scss">
.main{
    background: white;
    width: 100vw;
    height: 100vh;
    // margin-bottom: 3rem;
    .showdata{
        // margin-top: 1rem;
        padding-top: 3rem;
        background:violet;

    }
}
</style>