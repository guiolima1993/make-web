<template>
  <footer class="footer">
    <div class="footer-social">
      <a href="#">
        <img src="../assets/images/whatsapp.png" alt="Logo Whatssap">
      </a>
      <a href="#">
        <img src="../assets/images/instagram.png" alt="Logo Instagram">
      </a>
      <a href="#">
        <img src="../assets/images/facebook.png" alt="Logo Facebook">
      </a>
      <div class="footer-social-text">
        Todos os direitos reservados. Desenvolvido por: MakeWeb
      </div>
    </div>
    <div class="footer-contact">
      <div>
        <a href="#" class="footer-icon">
          <img src="../assets/images/phone.png" alt="Logo Facebook">
        </a>
      </div>
      <div>
        <p class="footer-text">
          <a href="#">(12) 3456-7890</a>
        </p>
      </div>
    </div>
    <div class="footer-mail">
      <div>
        <a href="#" class="footer-icon">
          <img src="../assets/images/mail.png" alt="Logo Facebook">
        </a>
      </div>
      <div>
        <p class="footer-text">
          <a href="mailto:email@email.com">email@email.com</a>
        </p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style lang="scss" scoped>
.footer {
  background: #C41520;
  display: flex;
  justify-content: center;
  position: relative;
  padding: 55px 0 0 0;

  &-social {
    text-align: center;
    margin-top: 10px;

    a {
      margin: 0 5px 0 5px;
    }

    &-text {
      color: #ffff;
      padding-top: 10px;
      font-size: 15px;
      margin-bottom: 10px;
    }
  }

  &-contact {
    display: flex;
    color: #fff;
    align-items: center;
    text-align: right;
    position: absolute;
    left: calc(50% - 29px/2 + 472.5px);
    top: 15%;
  }

  &-mail {
    display: flex;
    color: #fff;
    align-items: center;
    text-align: right;
    position: absolute;
    left: calc(50% - 29px/2 + 472.5px);
    top: 40%;
  }

  &-icon {
    margin-right: 14px;
  }

  &-text {
    font-size: 15px;

    a {
      text-decoration: none;
      color: #ffff;
      transition: all .6s;

      &:hover {
        color: #000;
      }
    }
  }
}
</style>