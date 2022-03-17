<template>
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
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="scss" scoped>
  .header {
  width: 100%;
  position: fixed;
  z-index: 1;
  display: flex;
  justify-content: space-between;
  padding: 0 10px;
  background: rgba(196, 21, 32, 0.7);
  text-align: center;
  

  &-logo {
    display: flex;
    align-items: center;

    a {
      margin-left: 42px;
      font-size: 30px;
      text-decoration: none;
      color: #fff;
      font-weight: 500;

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
          font-weight: 500;

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
      font-weight: 500;
      font-family: 'Mulish', sans-serif;

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
</style>