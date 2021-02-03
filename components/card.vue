<template>
    <div class="back">
        <div class="card">
            <div class="card_top">
                <div>หัวข้อโปรเจค</div>
                <div>10/10/10</div>
                <div><button></button></div>
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
.back{
    background: chartreuse;
    padding: 10px;
    .card{
        background: #DCD7D7;
        padding: 10px;
        width: fit-content;
        .card_top{
            display: flex;
            .card_top button{
                height: 100%;
                background-image: url("https://upload.wikimedia.org/wikipedia/commons/thumb/6/64/Edit_icon_%28the_Noun_Project_30184%29.svg/1024px-Edit_icon_%28the_Noun_Project_30184%29.svg.png");
            }
        }
    }
}
</style>