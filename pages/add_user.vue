<template>
    <div class="main">
        <add-user/>

    </div>
</template>

<script>
import add_user from '@/components/add_user'
export default {
    components:{
        add_user
    },
    data(){
        return
    }
}
</script>
<style lang="scss">
.main{
    background: chartreuse;
    width: 100vw;
    height: 100vh;
}  
</style>