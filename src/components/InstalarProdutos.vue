<template>
  <div class="install-products">
    <div class="install-products-content">
      <h1 class="install-products-content-title">Saiba como instalar nossos produtos</h1>
      <div>
        <select class="install-products-content-product">
          <option value="" disabled selected>Selecione o produto desejado</option>
        </select>
      </div>
      <div class="install-products-content-acess">
        <a href="#" class="install-products-content-acess-btn">Acessar</a>
      </div>
    </div>
  </div>
  <Footer />
</template>

<script>
import Footer from './Footer.vue'

export default {
  name: 'InstalarProdutos',
  components: {
    Footer
  }
}
</script>

<style lang="scss" scoped>
.install-products {
  margin-top: 74px;
  background-image: url('../assets/images/rectangle14.png');
  background-repeat: no-repeat;
  background-size: cover;
  padding: 38px 5px 53px 5px;

  &-content {
    width: 100%;
    text-align: center;
    color: #ffff;
    justify-content: center;

    &-title {
      font-size: 40px;
      text-transform: uppercase;
      font-weight: 300;

      @media (max-width: 880px) {
        font-size: 20px;
      }
    }

    &-product {
      width: 749px;
      padding: 10px 30px;
      margin: 0 20px;
      font-size: 25px;
      border: none;
      outline: none !important;
      border: 1px solid #EDEDED;
      color: #CECECE;
      box-sizing: border-box;
      border-radius: 5px;
      font-family: 'Mulish', sans-serif;
      appearance: none;
      background: #ffff url('../assets/images/vector.png') 95.66% 50% no-repeat;

      @media (max-width: 880px) {
        padding: 10px 20px;
        font-size: 15px;
        width: 500px;
      }

      @media (max-width: 530px) {
        width: 300px;
        margin: 0 5px;
      }
    }

    &-acess {
      margin-top: 38px;

      &-btn {
        padding: 13px 147px 15px 146px;
        font-size: 25px;
        border: 2px solid #C41520;
        box-sizing: border-box;
        border-radius: 5px;
        background: transparent;   
        color: #ffff;
        text-decoration: none;
        cursor: pointer;
        transition: all .6s;
        font-weight: 700;

        &:hover {
          background: rgba(196, 21, 32, 0.7);
        }

        @media (max-width: 470px) {
          padding: 13px 74px 15px 72px;
          font-size: 15px;
        }
      }
    }
  }
}
</style>