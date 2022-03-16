<template>
  <div class="products">
    <h1 class="products-title">Nossos Produtos</h1>
    <div class="products-section">
      <div class="products-section-left">
        <h1 class="products-section-left-title">
          Acessórios
        </h1>
        <div class="products-section-left-after"></div>
        <p class="products-section-left-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus facilis reprehenderit, ipsam minima sunt praesentium error maiores eum quibusdam, esse, corporis placeat explicabo exercitationem! Enim consequatur minus quia cum. Est.</p>
        <a href="#" class="products-section-left-link">Saiba mais</a>
      </div>
      <div class="products-section-left-img">
        <img src="../assets/images/unsplash_BQ5skcjX24o.png" alt="Imagem de Pessoa lavando a mão">
      </div>
    </div>
    <div class="products-section-second">
      <div class="products-section-second-img">
        <img src="../assets/images/cat2.png" alt="Imagem de Saboneteira">
      </div>
      <div class="products-section-right">
        <h1 class="products-section-left-title">
          Saboneteira
        </h1>
        <p class="products-section-left-text">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veritatis, consectetur! Voluptates aut, cumque quia minus perspiciatis, velit ratione perferendis sapiente ea ut et. Minus quas modi, nemo et inventore laborum.
        </p>
        <a href="#" class="products-section-left-link">Saiba mais</a>
      </div>
    </div>
    <div class="products-section">
      <div class="products-section-left">
        <h1 class="products-section-left-title">
          Outros
        </h1>
        <p class="products-section-left-text">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nobis deserunt nostrum obcaecati incidunt quas laborum aliquam vitae id velit itaque adipisci nulla vero temporibus consequatur et cupiditate, quod, fugiat cum!
        </p>
        <a href="#" class="products-section-left-link">Saiba mais</a>
      </div>
      <div class="products-section-left-img">
        <img src="../assets/images/cat1.png" alt="Imagem de Relógio">
      </div>
    </div>
  </div>
  <InstalarProdutos />
</template>

<script>
import InstalarProdutos from './InstalarProdutos.vue'

export default {
  name: 'Produtos',
  components: {
    InstalarProdutos
  }
}
</script>

<style lang="scss" scoped>
  .products {
    text-align: center;

    &-title {
      margin: 74px 0 0 0;
      padding: 0 10px;
      font-size: 80px;
      text-transform: uppercase;
      font-weight: 100;

      @media (max-width: 990px) {
        font-size: 40px;
      }
    }

    &-section {
      display: flex;
      align-items: center;
      padding: 0 102px 0 101px;
      margin-top: 100px;
      flex-direction: row;

      &-left {
        text-align: left;
        margin-right: 93px;

        &-title {
          font-size: 50px;
          text-transform: uppercase;
          margin: 0;
          font-weight: 100;

          @media (max-width: 990px) {
            font-size: 30px;
          }
        }

        &-text {
          font-size: 17px;
          font-weight: 100;
          margin: 30px 0;

          @media (max-width: 990px) {
            font-size: 10px;
          }
        }

        &-link {
          padding: 10px 20px;
          text-transform: uppercase;
          font-size: 25px;
          border: 1px solid #000;
          background: transparent;
          cursor: pointer;
          transition: all .6s;
          font-weight: 200;
          text-decoration: none;
          color: #000;

          &:hover {
            background: #e2e2e2;
          }

          @media (max-width: 990px) {
            padding: 5px 15px;
            font-size: 15px;
          }
        }

        @media (max-width: 990px) {
          text-align: center;
          margin: 0 0 30px 0;
          padding: 0 10px;
        }

        &-img {
          flex: 1 0 60%;
          text-align: right;

          img {
            max-width: 100%;
            max-height: 100%;
          }
        }
      }

      &-right {
        text-align: right;
        margin-left: 93px;

        @media (max-width: 990px) {
          text-align: center;
          margin: 0 0 30px 0;
          padding: 0 10px;
        }
      }

      @media (max-width: 990px) {
        flex-direction: column;
      }

      &-second {
        display: flex;
        align-items: center;
        padding: 0 102px 0 101px;
        margin-top: 100px;
        flex-direction: row;

        @media (max-width: 990px) {
          flex-direction: column-reverse;
        }

        &-img {
          flex: 1 0 60%;
          text-align: left;

          img {
            max-width: 100%;
            max-height: 100%;
          }
        }
      }
    }
  }
</style>