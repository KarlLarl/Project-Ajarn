<template>
  <div class="width100">
        <div class="test">
          <h4>FirstName</h4>
          <input placeholder="" type="text">
        </div>
        <div class="test">
            <h4>LastName</h4>
            <input placeholder="" type="text">
        </div>
        <div class="test">
            <h4>Email</h4>
            <input placeholder="" type="email">
        </div>
        <div class="test">
            <h4>Password</h4>
            <input placeholder="" type="password">
        </div>
        <div class="test">
            <h4>Comfirm Password</h4>
            <input placeholder="" type="password">
        </div>
        <div class="test">
            <h4>Phone</h4>
            <input placeholder="" type="number">
        </div>
  </div>
</template>
<style lang="scss" scoped>
h4{
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
    font-weight: bold;
    margin-left: 20px;
    width: 100%;
    }
    .test{
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
    }
@media screen and (max-width: 500px) /*จอเล็ก*/{
    .test{
    align-items: center;
    justify-content: space-between;
    width: 100%;
    flex-flow: wrap;
        }
    }
}

</style>