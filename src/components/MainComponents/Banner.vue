<template>
  <aside id="banner">
    <h1>Taay Beauty'n Care</h1>
  </aside>
</template>

<script>
export default {
  name: "Banner",
};
</script>
<style scoped>
@media (min-width: 375px) and (max-width: 800px) {
  #banner {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 300px;
    background-image: url(/public/img/banner.jpeg);
    background-size: cover;
    margin-bottom: 30px;
  }

  #banner h1 {
    text-align: center;
    color: white;
    font-size: 50px;
    text-shadow: 3px 3px 5px rgb(249, 164, 193), -3px -3px 5px #000;
    letter-spacing: 4px;
    font-family: "Great Vibes", cursive;
    font-weight: bold;
    font-style: normal;
  }
}

@media (min-width: 801px){
  #banner {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 400px;
    background-image: url(/public/img/banner.jpeg);
    background-size: cover;
    margin-bottom: 30px;
  }

  #banner h1 {
    text-align: center;
    color: white;
    font-size: 100px;
    text-shadow: 3px 3px 5px rgb(245, 51, 116), -3px -3px 5px #000;
    letter-spacing: 4px;
    font-family: "Great Vibes", cursive;
    font-weight: bold;
    font-style: normal;
  }

}
</style>