<script>
import inizio from './components/headerComponent.vue';
import fine from './components/footerComponent.vue';
export default {
  name: `corpo`,
  components: {
    inizio,
    fine,
  },
};
</script>
<template>
  <!-- header -->
  <inizio />

      <!--main-->
      <main>
          <div class="container">
              <div class="wrap">
                  <div class="content">
                      <img class="prodotti" src="./components/img/1.webp" alt="img-1">
                      <img class="hover-image" src="./components/img/1b.webp" alt="img-1b">
                      <div class="col red">-50%</div>
                      <div class="right-1 col green">Sostenibilità</div>
                      <div class="cuore"> <i class="fa-solid fa-heart"></i></div>
                      <p class="piccolo">Levi's</p>
                      <strong class="testo">RELAXED FIT TEE UNISEX</strong>
                      <p class="numeri">14,99 &euro; <del>29,99 &euro;</del> </p>
                  </div>
                  <div class="content">
                      <img class="prodotti" src="./components/img/2.webp" alt="img-2">
                      <img class="hover-image" src="./components/img/2b.webp" alt="img-2b">
                      <div class="col red">-30%</div>
                      <div class="cuore"> <i class="fa-solid fa-heart"></i></div>
                      <p class="piccolo">Guess</p>
                      <strong class="testo">ROSES TEE</strong>
                      <p class="numeri">20,99 &euro; <del>29,99 &euro;</del></p>
                  </div>
                  <div class="content">
                      <img class="prodotti" src="./components/img/3.webp" alt="img-3">
                      <img class="hover-image" src="./components/img/3b.webp" alt="img-3b">
                      <div class="col red">-30%</div>
                      <div class="cuore"> <i class="fa-solid fa-heart"></i></div>
                      <p class="piccolo">Come Zucchero Filato</p>
                      <strong class="testo">VOGLIA DI COLORI PASTELLO</strong>
                      <p class="numeri">129,99 &euro; <del>184,99 &euro;</del></p>
                  </div>
                  <div class="content">
                      <img class="prodotti" src="./components/img/4.webp" alt="img-4">
                      <img class="hover-image" src="./components/img/4b.webp" alt="img-4b">
                      <div class="col red">-50%</div>
                      <div class="right-1 col green">Sostenibilità</div>
                      <div class="cuore"> <i class="fa-solid fa-heart"></i></div>
                      <p class="piccolo">Levi's</p>
                      <strong class="testo">TEE UNISEX</strong>
                      <p class="numeri">14,99 &euro; <del>29,99 &euro;</del></p>
                  </div>
                  <div class="content">
                    
                      <img class="prodotti" src="./components/img/5.webp" alt="img-5">
                      <img class="hover-image" src="./components/img/5b.webp" alt="img-5b">
                      <div class="cuore"> <i class="fa-solid fa-heart"></i></div>
                      <p class="piccolo">Maya Deluxe</p>
                      <strong class="testo">STRIPE BODICE</strong>
                      <p class="numeri">99,99 &euro;</p>
                  </div>
                  <div class="content">
                      <img class="prodotti" src="./components/img/6.webp" alt="img-6">
                      <img class="hover-image" src="./components/img/6b.webp" alt="img-6b">
                      <div class="col green">Sostenibilità</div>
                      <div class="cuore"> <i class="fa-solid fa-heart"></i></div>
                      <p class="piccolo">Esprit</p>
                      <strong class="testo">MAGLIONE - BLACK</strong>
                      <p class="numeri">29,99 &euro;</p>
                  </div>
              </div>
          </div>
      </main>
      <!-- footer -->
      <fine />

</template>
<style lang="scss">
@mixin font($size){
  font-size: $size;
}
%position{
  padding: 5px 6px;
  position: absolute;
  bottom: 28%;
}
main{
  padding: 5rem;
  .wrap{
    display: flex;
    flex-wrap: wrap;
  }
  .content{
      position: relative;
      padding-bottom: 60px;
  }
  .prodotti{
      width: 380px;
      margin-right: 20px;
  }
  .piccolo{
      @include font(10px)
  }
  .testo{
      @include font(10px)
  }
  .numeri{
      color: red;
      font-size: 12px;
  }
  del{
      color: black;
  }
  .content:hover .prodotti{
      display: none;
  }
  .content:hover .hover-image{
      display: block;
  }
  .hover-image{
      display: none;
      width: 380px;
      position: relative;
      margin-right: 20px;
  }
  .cuore{
      background-color: white;
      color: black;
      position: absolute;
      top: 15px;
      right: 20px;
      padding: 5px 10px;
  }
  .col{
      color: white;
  }
  .red{
      @extend %position;
      background-color: red;
      
  }
  .green{
      @extend %position;
      background-color: green;
  }
  .right-1{
      left: 55px;
  }
}
</style>