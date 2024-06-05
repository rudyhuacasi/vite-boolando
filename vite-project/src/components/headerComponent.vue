<script>
  
</script>
<template>
  <!--header-->
      <header>
          <div class="container">
              <div class="d-flex">
                  <div class="small">
                      <p> Donna  Uomo  Bambini </p>
                  </div>
                  <div class="large">
                      <img class="boolean" src="./img/boolean-logo.png" alt="">
                  </div>
                  <div class="small icona">
                      <i class="fa-regular fa-user"></i>
                      <i class="fa-regular fa-heart"></i>
                      <i class="fa-solid fa-bag-shopping"></i>
                  </div>
              </div>
          </div>
      </header>
</template>

<style lang="scss">

%message-shared {
  width: 20%;
  color: white;
}

header{
    background-color: rgb(253, 114, 0);
    height: 70px;
    display: flex;
    align-items: center;
    position: fixed;
    width: 100%;
    z-index: 20;
    border-bottom: 1px solid silver;

  .d-flex{
    display: flex;
    align-items: center;
  }

  .small{
    @extend %message-shared;
  }

  .large{
    width: 60%;
    text-align: center;
  }

  .boolean{
    width: 180px;
  }

  .icona{
    @extend %message-shared;
    text-align: right;
  }
  
}
i{
    padding: 5px;
  }
</style>