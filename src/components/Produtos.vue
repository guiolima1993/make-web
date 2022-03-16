<template>
  <div class="products">
    <h1 class="products-title">Nossos Produtos</h1>
    <div class="products-section-accessories">
      <div class="products-section-accessories-left">
        <h1 class="products-section-accessories-left-title">
          Acessórios
        </h1>
        <div class="products-section-accessories-left-after"></div>
        <p class="products-section-accessories-left-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ducimus facilis reprehenderit, ipsam minima sunt praesentium error maiores eum quibusdam, esse, corporis placeat explicabo exercitationem! Enim consequatur minus quia cum. Est.</p>
        <button class="products-section-accessories-left-btn">Saiba mais</button>
      </div>
      <div class="products-section-accessories-rigth">
        <img src="../assets/images/unsplash_BQ5skcjX24o.png" alt="Imagem de Pessoa lavando a mão">
      </div>
    </div>
    <div class="products-section-soap-dish">
      <div class="products-section-soap-dish-left">
        <img src="../assets/images/cat2.png" alt="Imagem de Saboneteira">
      </div>
      <div class="products-section-soap-dish-right">
        <h1 class="products-section-soap-dish-right-title">
          Saboneteira
        </h1>
        <p class="products-section-soap-dish-right-text">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veritatis, consectetur! Voluptates aut, cumque quia minus perspiciatis, velit ratione perferendis sapiente ea ut et. Minus quas modi, nemo et inventore laborum.
        </p>
        <button class="products-section-soap-dish-right-btn">Saiba mais</button>
      </div>
    </div>
    <div class="products-section-others">
      <div class="products-section-others-left">
        <h1 class="products-section-others-left-title">
          Outros
        </h1>
        <p class="products-section-others-left-text">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nobis deserunt nostrum obcaecati incidunt quas laborum aliquam vitae id velit itaque adipisci nulla vero temporibus consequatur et cupiditate, quod, fugiat cum!
        </p>
        <button class="products-section-others-left-btn">Saiba mais</button>
      </div>
      <div class="products-section-others-right">
        <img src="../assets/images/cat1.png" alt="Imagem de Relógio">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Produtos'
}
</script>

<style lang="scss" scoped>
  .products {
    text-align: center;

    &-title {
      margin-top: 74px;
      font-size: 80px;
      text-transform: uppercase;
    }

    &-section-accessories {
      display: flex;
      align-items: center;
      padding: 0 102px 0 101px;

      &-left {
        text-align: left;
        margin-right: 93px;

        &-title {
          font-size: 50px;
          text-transform: uppercase;
          margin: 0;
        }

        &-text {
          font-size: 17px;
        }

        &-btn {
          padding: 10px 20px;
          text-transform: uppercase;
          font-size: 25px;
          border: 1px solid #000;
          background: transparent;
          cursor: pointer;
          transition: all .6s;

          &:hover {
            background: #e2e2e2;
          }
        }
      }
    }

    &-section-soap-dish {
      margin-top: 100px;
      display: flex;
      align-items: center;
      padding: 0 102px 0 101px;

      &-right {
        text-align: right;
        margin-left: 93px;

        &-title {
          font-size: 50px;
          text-transform: uppercase;
          margin: 0;
        }

        &-text {
          font-size: 17px;
        }

        &-btn {
          padding: 10px 20px;
          text-transform: uppercase;
          font-size: 25px;
          border: 1px solid #000;
          background: transparent;
          cursor: pointer;
          transition: all .6s;

          &:hover {
            background: #e2e2e2;
          }
        }
      }
    }

    &-section-others {
      margin-top: 100px;
      display: flex;
      align-items: center;
      padding: 0 102px 0 101px;

      &-left {
        text-align: left;
        margin-right: 93px;

        &-title {
          font-size: 50px;
          text-transform: uppercase;
          margin: 0;
        }

        &-text {
          font-size: 17px;
        }

        &-btn {
          padding: 10px 20px;
          text-transform: uppercase;
          font-size: 25px;
          border: 1px solid #000;
          background: transparent;
          cursor: pointer;
          transition: all .6s;

          &:hover {
            background: #e2e2e2;
          }
        }
      }
    }
  }
</style>