<template>
  <section id="cards">
    <div id="card" v-for="(item, index) in imagens" :key="index">
      <p>Produto</p>
      <figure><img :src="item.imagem" :alt="item.name" /></figure>
      <span>{{ item.preco }}</span>
    </div>
  </section>
</template>

<script>
export default {
  name: "cardsProdutos",
  data() {
    return {
      imagens: [
        { index: 0, imagem: "/img/produto-1.png", name: "Produto 1", preco: 0 },
        { index: 1, imagem: "/img/produto-2.png", name: "Produto 2", preco: 0 },
        { index: 2, imagem: "/img/produto-3.png", name: "Produto 3", preco: 0 },
        { index: 3, imagem: "/img/produto-4.png", name: "Produto 4", preco: 0 },
        { index: 4, imagem: "/img/produto-5.png", name: "Produto 5", preco: 0 },
        { index: 5, imagem: "/img/produto-6.png", name: "Produto 6", preco: 0 },
        { index: 6, imagem: "/img/produto-7.png", name: "Produto 7", preco: 0 },
        { index: 7, imagem: "/img/produto-8.png", name: "Produto 8", preco: 0 },
        { index: 8, imagem: "/img/produto-9.png", name: "Produto 9", preco: 0 },
        {
          index: 9,
          imagem: "/img/produto-10.png",
          name: "Produto 10",
          preco: 0,
        },
        {
          index: 10,
          imagem: "/img/produto-11.png",
          name: "Produto 11",
          preco: 0,
        },
        {
          index: 11,
          imagem: "/img/produto-12.png",
          name: "Produto 12",
          preco: 0,
        },
      ],
    };
  },
};
</script>

<style scoped>
@media (min-width: 375px) and (max-width: 800px) {
  #cards {
    display: flex;
    justify-content: center;
    align-items: center;
    width: calc(100% - 30px);
    flex-wrap: wrap;
    gap: 10px;
  }

  #card {
    width: 300px;
    height: 400px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    background-color: rgb(249, 164, 193);
    border-radius: 10px;
    letter-spacing: 2px;
    flex-grow: 0;
    flex-basis: 1;
  }

  #card p {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 50px;
    font-size: 23px;
    color: #fff;
    text-shadow: 1.5px 1.5px black;
  }

  #card figure {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 90%;
    height: 300px;
    overflow: hidden;
    background-color: #fff;
    border-radius: 30px;
  }

  #card figure img {
    margin-top: 5px;
    width: 70%;
  }

  #card span {
    width: 100%;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 23px;
    color: #fff;
    text-shadow: 1.5px 1.5px black;
  }
}

@media (min-width: 801px) {
  #cards {
    display: flex;
    justify-content: center;
    align-items: center;
    width: calc(100% - 30px);
    flex-wrap: wrap;
    gap: 10px;
  }

  #card {
    width: 300px;
    height: 400px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    background-color: rgb(249, 164, 193);
    border-radius: 10px;
    letter-spacing: 2px;
    flex-grow: 0;
    flex-basis: 1;
  }

  #card p {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 50px;
    font-size: 23px;
    color: #fff;
    text-shadow: 1.5px 1.5px black;
  }

  #card figure {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 90%;
    height: 300px;
    overflow: hidden;
    background-color: #fff;
    border-radius: 30px;
  }

  #card figure img {
    margin-top: 5px;
    width: 70%;
  }

  #card span {
    width: 100%;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 23px;
    color: #fff;
    text-shadow: 1.5px 1.5px black;
  }
}
</style>