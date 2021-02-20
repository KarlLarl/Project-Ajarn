<template>
<div class="background">
    <nevbar/>
    TEST


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
.background{
    background: blueviolet;
    width: 100vw;
    height: 100vh;
    padding-top: 3rem;
}
</style>