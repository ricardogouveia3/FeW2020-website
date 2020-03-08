<template>
  <div class="header">
    <div class="header__content">
      <img
        src="../assets/icons/sp_state-white.svg"
        alt="Ícone representando o estado de São Paulo"
        class="header__content__icon"
      />
      <h1 class="header__content__title">Front-end Week <br>SP <span>#2020</span></h1>
      <p class="header__content__date">De 13 a 18 de Julho</p>
      <button class="header__content__button">
        Programação
        <img src="../assets/icons/arrow_right_blue.svg" alt="Seta apontando para direita" />
      </button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.header {
  overflow: visible;
  background-color: rgba(4, 33, 73, 0.9);
  font-family: "Montserrat", sans-serif;
  height: 100%;
  width: 33%;
  display: flex;
  align-items: center;
  padding-left: 50px;
}

.header__content {
  text-align: left;
  white-space: nowrap;
}

h1 {
  font-size: 60px;
  text-transform: uppercase;
  font-weight: bold;
  margin: 10px 0;

  span {
    font-weight: 300;
    color: #4A90E2;
  }
}

p {
  font-size: 25px;
}

button {
  color: #4A90E2;
  font-weight: 600;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 250px;
  height: 50px;
  border: none;
  border-radius: 50px;
  cursor: pointer;
  font-size: 21px;
  box-shadow: 0 2px 3px rgba(0, 0, 0, 0.2) ;

  img {
    margin-left: 10px;
    width: 15px;
  }
}

</style>
