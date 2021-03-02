<template>
    <div >
        <div class="card" >
            <div class="into_card">
                <a onclick="window.location.href='/show'">
                    <div class="card_img"></div>
                    <div class="card_deteil">
                        <div class="info_card">
                            <Label class="card_name" v-model="card_Name">{{cardName}}</Label>
                            <Label class="card_date" v-model="card_Date">{{cardDate}}</Label>
                        </div>
                        
                    </div>
                    
                </a>
            </div>
            
        </div>
    </div>    
</template>

<script>
export default {
    props:['cardName','cardDate'],
    data(){
        return {

        }
    }
    
}
</script>

<style lang="scss" scoped>
.card{
    // background: cadetblue;
    width: 14rem;
    height: 14rem;
    padding: 10px;
    

    .into_card{
        // border: 1px solid black; 
        height: 100%; 
        border-radius: 5px;
        box-shadow: 5px 5px 10px 5px rgba(224,224,224,0.5);
        transition: 0.4s ease-out;
        &:hover {
        box-shadow: 0 0 6px 6px rgba(0, 0, 0, 0.6);
        }
        .card_img{
            height: 70%;
            width: 100%;
            border-radius: 5px 5px 0 0;
            background-size: 100% 100%;
            background-image: url("https://img.freepik.com/free-vector/hexagonal-technology-pattern-mesh-background-with-text-space_1017-26293.jpg?size=626&ext=jpg");
        }
        .card_deteil{
            height: 30%;
            background: white;
            border-radius: 0 0 5px 5px;
            .info_card{
                display: flex;
                flex-direction: column;
                text-align: left;
                padding: 10px;
                .card_date{
                    font-size: 10px;
                }
                // .btn_git{
                //     display: flex;
                //     justify-content: flex-end;
                // }
            }
        }
    }

}
</style>