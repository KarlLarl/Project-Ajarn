<template>
  <div class="width100">
        <div class="test">
          <label>FirstName</label>
          <input placeholder="" type="text">
        </div>
        <div class="test">
            <label>LastName</label>
            <input placeholder="" type="text">
        </div>
        <div class="test">
            <label>Email</label>
            <input placeholder="" type="email">
        </div>
        <div class="test">
            <label>Password</label>
            <input placeholder="" type="password">
        </div>
        <div class="test">
            <label>Comfirm Password</label>
            <input placeholder="" type="password">
        </div>
        <div class="test">
            <label>Phone</label>
            <input placeholder="" type="number">
        </div>
  </div>
</template>
<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css?family=Prompt:100,200,400,500,600,700&display=swap');

*{font-family: 'Prompt', sans-serif;}

$wd100:100%;
label{
    width: 30%;
}
.width100{
    // width: 100%;
    display: flex;
    flex-direction: column;
    input {
    padding: 12px 20px;
    border: none;
    background-color: #F5EBEB;
    border-radius: 10px;
    margin-top: 10px;
    // font-weight: bold;
    margin-left: 20px;
    width: $wd100;
    }
    .test{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: $wd100;
    }
@media screen and (max-width: 500px) /*จอเล็ก*/{
    .test{
    align-items: center;
    justify-content: space-between;
    width: $wd100;
    flex-flow: wrap;
        }
    }
}

</style>