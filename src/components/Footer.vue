<template>
  <footer>
    <p>Desenvolvido por <span>Speller - Dev</span></p>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
footer {
  width: 100%;
  height: 100px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: rgb(249, 164, 193);
  margin-top: 30px;
  font-size: 25px;
}

footer p {
  color: #fff;
  letter-spacing: 2px;
  text-shadow: 0px 0px black, -2px -2px black;
}

footer span {
  font-family: "Honk", system-ui;
  font-optical-sizing: auto;
  font-weight: 400;
  font-style: normal;
  font-variation-settings: "MORF" 15, "SHLN" 50;
  letter-spacing:  5px;
  font-size: 30px;
}
</style>
