<template>
  <header id="header">
    <router-link to="/">
      <figure id="logo">
        <img src="/img/logo.png" alt="Logo Taay Beauty Care" />
      </figure>
    </router-link>

    <nav id="nav">
      <button @click="MenuColapsed">
        <img :src="altearImagem" alt="Menu" />
      </button>
      <ul v-show="visivel">
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/produtos">Produtos</router-link></li>
      </ul>
      <ul id="menu">
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/produtos">Produtos</router-link></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      altearImagem: "/img/open-menu.png",
      visivel: false,
    };
  },
  methods: {
    MenuColapsed() {
      if (
        this.visivel === false &&
        this.altearImagem === "/img/open-menu.png"
      ) {
        this.visivel = true;
        this.altearImagem = "/img/closed-menu.png";
      } else {
        this.visivel = false;
        this.altearImagem = "/img/open-menu.png";
      }
    },
  },
};
</script>

<style scoped>
@media (min-width: 375px) and (max-width: 800px) {
  #header {
    width: 100%;
    height: 15vh;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    background-color: rgb(249, 164, 193);
  }
  #logo {
    width: 150px;
  }

  #logo img {
    width: 100px;
  }

  #nav {
    display: flex;
    position: absolute;
    right: -150px;
    top: 0;
  }
  #nav button {
    border-style: none;
    background-color: transparent;
  }

  #nav ul {
    width: 150px;
    height: 150px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  #nav ul li {
    padding: 10px 60px;
    color: #fff;
  }

  #nav ul li a {
    color: #fff;
    font-size: 20px;
  }

  #menu li {
    display: none;
  }
}

@media (min-width: 801px) {
 #header {
    width: 100%;
    height: 20vh;
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: rgb(249, 164, 193);
    border-bottom: 2px solid rgba(238, 85, 136, 0.623);
  }
  #logo {
    width: 150px;
  }

  #logo img {
    margin-left: 20%;
    width: 150px;
  }

  #nav {
    display: flex;
 

  }
  #nav button {
    display: none;
    border-style: none;
    background-color: transparent;
  }

  #nav ul {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  #nav ul li {
    padding: 10px 60px;
    color: #fff;
  }

  #nav ul li a {
    color: #fff;
    font-size: 20px;
  }
}
</style>