<template>
  <div class="main-banner">
    <header class="header">
      <div class="header-logo">
        <a href="#">Empresa</a>
      </div>
      <div class="header-nav-menu">
        <ul class="header-nav-menu-list">
          <li class="header-nav-menu-list-item"><a href="#">Home</a></li>
          <li class="header-nav-menu-list-item"><a href="#">Empresa</a></li>
          <li class="header-nav-menu-list-item"><a href="#">Produtos</a></li>
          <li class="header-nav-menu-list-item"><a href="#">Notícias</a></li>
          <li class="header-nav-menu-list-item"><a href="#">Contato</a></li>
          <li class="header-nav-menu-list-item"><button class="header-nav-menu-btn">Loja Online</button></li>
        </ul>
      </div>
    </header>
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
        <h3 class="main-banner-title-project">Design</h3>
        <h1 class="main-banner-title-modern">Moderno</h1>
        <div class="main-banner-title-line">

        </div>
        <p class="main-banner-title-text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Cum placeat quaerat, tempora quibusdam possimus omnis, ratione exercitationem nostrum, excepturi eligendi repellendus corrupti. Quis qui repellat minima deleniti! Quibusdam, enim illo.</p>
      </div>
    </div>
  </div>
  <Produtos />
</template>

<script>
import Produtos from './Produtos.vue'

export default {
  name: 'HelloWorld',
  components: {
    Produtos
  }
}
</script>


<style scoped lang="scss">
.header {
  width: 100%;
  position: fixed;
  z-index: 1;
  display: flex;
  justify-content: space-between;
  padding: 0 10px;
  background: rgba(196, 21, 32, 0.7);
  

  &-logo {
    display: flex;
    align-items: center;

    a {
      margin-left: 42px;
      font-size: 30px;
      text-decoration: none;
      color: #fff;

      &:hover {
        color: #000;
        transition: all .6s;
      }

      @media (max-width: 1005px) {
      margin: 0;
      } 
    }

    @media (max-width: 1005px) {
      display: block;
    }
  }

  &-nav-menu {
    margin-right: 40px;
    font-size: 30px;

    &-list {
      list-style: none;
      display: flex;
      justify-content: center;
      align-items: center;

      &-item {
        a {
          margin-left: 25px;
          text-decoration: none;
          color: #fff;

          &:hover {
            color: #000;
            transition: all .6s;
          }

          @media (max-width: 1005px) {
            margin: 0;;
          }
        }
      }

      @media (max-width: 1005px) {
        display: block;
        font-size: 20px;
        margin: 10px 0 0 0;
        padding: 0;
      }
    }

    &-btn {
      margin-left: 25px;
      border-radius: 10px;
      width: 178px;
      height: 57px;
      cursor: pointer;
      border: none;
      font-size: 30px;
      color: #C41520;

      &:hover {
        border: 1px solid #000;
        box-shadow: 1px 2px 5px #000;
        color: #ff1423;
      }

      @media (max-width: 1005px) {
        margin: 10px 0 0 0;
        width: 100px;
        height: 27px;
        font-size: 15px;
      }
    }

    @media (max-width: 1005px) {
      display: block;
      margin: 0;
    }
  }

  @media (max-width: 1005px) {
    display: block;
    margin: 0;
    padding: 30px 0;
  }
}

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
      margin: 0;
      position: absolute;
      top: 310px;
      color: #ffff;
      text-transform: uppercase;

      &-project {
        font-size: 40px;
        margin: 0;
      }

      &-modern {
        font-size: 80px;
        margin: -20px 0 0 0;

        @media (max-width: 430px) {
          font-size: 55px;
        }
      }

      &-line {
        width: 100%;
        max-width: 50px;
        border: 2px solid #C41520;
        position: absolute;
        left: 32%;
        margin-top: -15px;
        transform: rotate(-179.29deg);
      }

      &-text {
        padding: 0 336px;
        margin: 0;

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
