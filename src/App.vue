<script>
export default {
  data() {
    return {
      contador: 0,
    };
  },
  methods: {
    sumarUno() {
      this.contador = this.contador + 1;
    },
    restarUno() {
      this.contador = this.contador - 1;
    },
    resetcount() {
      this.contador = 0;
    },
  },
};
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="" width="125" height="125" />
    <small><h1>Hola Mundo desde vue.js 3</h1></small>
    <hr />

    <h2>contador: {{ contador }}</h2>
    <button @click="sumarUno()">+1</button>
    <button @click="restarUno()">-1</button>
    <button @click="resetcount()">reset</button>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
}
small {
  color: #666;
}

h1 {
  font-weight: bolder;
}
h2 {
  font-size: 2.5rem;
}
button {
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 6px;
}
</style>
