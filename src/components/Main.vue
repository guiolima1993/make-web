<template>
  <Header />  
  <div class="main-banner">
    <div class="main-banner-icon">
      <a href="#">
        <img src="../assets/images/whats.png" alt="Logo Whatsapp">
      </a>
    </div>
    <div class="container">
      <div class="main-banner-img">
        <img class="main-banner-content" src="../assets/images/banner.png" alt="Imagem de Banheiro">
      </div>
      <div class="main-banner-title">
        <div class="main-banner-title-modern">
          <h3 class="main-banner-title-modern-project">Design</h3>
          <h1>Moderno</h1>
        </div>
        <p class="main-banner-title-text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Cum placeat quaerat, tempora quibusdam possimus omnis, ratione exercitationem nostrum, excepturi eligendi repellendus corrupti. Quis qui repellat minima deleniti! Quibusdam, enim illo.</p>
      </div>
    </div>
  </div>
  <Produtos />
</template>

<script>
import Produtos from './Produtos.vue'
import Header from './Header.vue'

export default {
  name: 'HelloWorld',
  components: {
    Header, Produtos
  }
}
</script>


<style scoped lang="scss">
.main-banner {
  text-align: center;
  
  &-img {
    animation: show 6s;

    img {
      width: 100%;
      height: 100vh;
    }
  }

  &-title {
    display: block;
    width: 100%;
    margin: 0;
    position: absolute;
    top: 310px;
    color: #ffff;
    text-transform: uppercase;

    &-modern {
      text-align: left;
      display: inline-block;

      &-project {
        font-size: 40px;
        margin: 0;
        font-weight: 100;
        letter-spacing: 2px;
        text-align: center;
        line-height: 90%;
      }

      h1 {
        letter-spacing: 2px;
        font-size: 80px;
        font-weight: 200;
        margin: 0;
        line-height: 80%;

        @media (max-width: 430px) {
          font-size: 55px;
        }
      }

      &::after {
        content: "";
        width: 50px;
        display: inline-block;
        background: #C41520;
        height: 6px;
      } 
    }

    &-text {
      padding: 0 336px;
      margin: 10px 0 0 0;
      font-weight: 100;

      @media (max-width: 1005px) {
        padding: 0 30px;
      }
    }

    @media (max-width: 1005px) {
      top: 400px;
    }
  }

  &-icon {
    position: fixed;
    right: 0;
    top: 50%;
    z-index: 1;
    margin: 0;
    padding: 0;
  }
}

  @keyframes show {
    0% {
        transform: scaleZ(100%);
    }
    25% {
        transform: scale(110%);
    }
    50% {
      transform: scale(130%);
    }
    100% {
        transform: scale(100%);
    }
}
</style>
