<template>
  <div>
    <!-- ถ้าหน้า login -->
    <div v-if="path === 'login'">
      <div><input class="in_log" placeholder="Email" type="text"></div>
      <div><input class="in_log" placeholder="Password" type="password"></div>
    </div>
    <!-- ถ้าหน้า topic -->
    <div v-if="path === 'create_topic'" class="detail">
            <div class="create_top">
                <label class="top_name">สร้างหัวข้อ</label>
            </div>
            <!-- ข้อมูลการกรอก -->
            <div class="input_info">
                <div class="left">
                    หัวข้อโปรเจค :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>

            <div class="input_info">
                <div class="left">
                    อาจารย์ที่ปรึกษาโปรเจค :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>

            <div class="input_info">
                <div class="left">
                    วัน/เดือน/ปี :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>

            <div class="input_info">
                <div class="left">
                    Github/Gitlab :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>
    </div>
    <!-- ถ้าหน้า appointment -->
    <div v-if="path === 'appointment'" class="detail">
            <div class="create_top">
                <label class="top_name">สร้างนัดหมาย</label>
            </div>
            <!-- ข้อมูลการกรอก -->
            <div class="input_info">
                <div class="left">
                    เรื่องที่นัดหมาย :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>

            <div class="input_info">
                <div class="left">
                    วัน/เดือน/ปี :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>

            <div class="input_info">
                <div class="left">
                    เวลา :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>
    </div>
    <!-- ถ้าหน้า progress_page -->
    <div v-if="path === 'progress_page'" class="detail">
            <div class="create_top">
                <label class="top_name">รายงานความคีบหน้า</label>
            </div>
            <!-- ข้อมูลการกรอก -->
            <div class="input_info">
                <div class="left">
                    เรื่อง :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>

            <div class="input_info">
                <div class="left">
                    วัน/เดือน/ปี :
                </div>

                <div class="right">
                    <input class="input_right" type="text">
                </div>
            </div>

            <div class="input_info">
                <div class="left">
                    Design :
                </div>

                <div>
                    <input  type="file">
                </div>
            </div>
    </div>

  </div>
</template>
<script>
export default {
  data(){
        return{
            path: ''
              }
  },
  mounted(){
        this.path = this.$route.name
    } 
  }
</script>
<style lang="scss" scoped>
.in_log {
  width: 100%;
  padding: 12px 20px;
  border: none;
  background-color: #F5EBEB;
  border-radius: 10px;
  margin-top: 10px;
  font-weight: bold;
}
.detail{
        .create_top{
            // background: chartreuse;
            text-align: center;
            padding: 10px;
            padding-bottom: 3rem;
            .top_name{
                // font-weight: bold;
                font-size: 28px;
            }
        }
        .input_info{
            // background: red;
            display: flex;
            width: 100%;
            padding-bottom: 20px;
            .left{
                width: 50%;
                padding-left: 20rem;
                flex-direction: column;
                justify-content: center;
                display: flex;
            }
            .right{
                width: 50%;
                .input_right{
                    background: #F5EBEB;
                    border-radius: 7px;
                    border: 1px solid black;
                    padding: 10px;
                    width: 75%;
                }
            }
        }  
}
</style>