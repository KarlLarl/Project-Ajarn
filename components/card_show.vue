<template>
    <div>
        <div class="card" >
            <div class="into_card">
                <a onclick="window.location.href='/show'">
                    <div class="card_img"></div>
                    <div class="card_deteil">
                        <div class="info_card">
                            <Label class="card_name">Name</Label>
                            <Label class="card_date">10/20/2010</Label>
                        </div>
                    </div>
                </a>
            </div>
            
        </div>
    </div>    
</template>

<script>
export default {
    // props:['imgCard','cardName','cardDate'],
    data(){
        return {
        }
    }
    
}
</script>

<style lang="scss" scoped>
.card{
    // background: cadetblue;
    width: 240px;
    height: 240px;
    padding: 10px;
    
    .into_card{
        // border: 1px solid black; 
        height: 100%; 
        border-radius: 5px;
        box-shadow: 5px 5px 5px 0 rgba(224,224,224,0.5); 
        .card_img{
            height: 70%;
            width: 100%;
            border-radius: 5px 5px 0 0;
            background-size: 100% 100%;
            background-image: url("https://img.rawpixel.com/s3fs-private/rawpixel_images/website_content/v462-n-130-textureidea_1.jpg?w=800&dpr=1&fit=default&crop=default&q=65&vib=3&con=3&usm=15&bg=F4F4F3&ixlib=js-2.2.1&s=9465282a2b0a375f4f5b120d7bbad882");
        }
        .card_deteil{
            height: 30%;
            .info_card{
                display: flex;
                flex-direction: column;
                text-align: left;
                padding: 10px;
                .card_date{
                    font-size: 10px;
                }
            }
        }
    }

}
</style>