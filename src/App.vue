<template>
  <div id="app">
    <h2>Botones</h2>
    <botones class="com_boton botones1"/>
    <botones class="com_boton botones2"/>
    <botones class="com_boton botones3"/>
    <botones class="com_boton botones4"/>
    <botonesDis class="com_boton botones5"/>
    <btnCompra class="com_boton botones6"/>
    <botones class="com_boton botones7"/>
    <bariosBtn class="com_boton botones8"/>
    <bariosBtn class="com_boton botones8 btnHover"/>
    <footer>
      <div class="iconos">
        <p>Icono: https://boxicons.com/</p>
      </div>
      <div class="castel">
        Esteban Javier Castelblanco Garcia
      </div>
    </footer>
  </div>
</template>

<script>

  import botones from "./components/botones.vue"
  import botonesDis from "./components/botonDis.vue"
  import btnCompra from "./components/botonCompra.vue"
  import bariosBtn from "./components/barios-btn.vue"

export default {
  name: 'App',
  components: {
    botones,
    botonesDis,
    btnCompra,
    bariosBtn
  }
}
</script>

<style>

  *{
    margin: 0;
    padding: 0;
  }

  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    width: 70%;
    margin: auto;
    margin-top: 60px;
  }

  .com_boton{
    margin-top: 60px;
  }

  .com_boton > button{
    cursor: pointer;
  }

  .botones1 > .btn2:hover{
    background-color: #999;
  }

  .botones1 > .btn2:focus{
    background-color: #888;
  }

  .botones2 > button{
    background-color: #fff;
    color: #04f;
    border: 1px solid #04f;
  }

  .botones2 > .btn2:hover, .botones3 > .btn2:hover{
    background: #04f2;
  }

  .botones2 > .btn2:focus, .botones3 > .btn2:focus{
    background-color: #04f1;
  }

  .botones3 > button{
    background-color: transparent;
    color: #04f;
  }

  .botones4 > button{
    background-color: #04f;
    color: #fff;
  }

  .botones4 > .btn2:hover{
    display: none;
  }

  .botones5 > .btn2:hover{
    background-color: transparent;
    cursor: default;
  }

  .botones6 > button{
    display: flex;
    align-items: center;
    background-color: #04f;
    color: #fff;
    padding: 17px 8px;
  }

  .botones6 > button > span{
    margin-left: 10px;
  }

  .botones6 > button > img{
    margin-left: 10px;
  }

  .botones6 > .btn2:hover{
    display: flex;
    flex-flow: row-reverse;
  }

  .botones7 > button{
    background-color: #04f;
    color: #fff;
  }

  .botones7 > .btn2:hover{
    padding: 18px 25px;
  }

  .botones7 > .btn2:focus{
    padding: 20px 30px;
  }

  .botones8 > .btn2{
    background-color: #04f;
    color: #fff;
  }

  .botones8 > .btn3{
    background-color: #555;
    color: #fff;
  }

  .botones8 > .btn4{
    background: #d32f2f;
    color: #fff;
  }

  .btnHover > .btn1:hover{
    background-color: #999;
  }

  .btnHover > .btn2:hover{
    background-color: #00f;
  }

  .btnHover > .btn3:hover{
    background-color: #333;
  }

  .btnHover > .btn4:hover{
    background-color: #a00;
  }


  footer{
    margin: 60px 0 30px 0;
    color: #aaa;
  }

  .iconos{
    margin-bottom: 100px;
  }

  .castel{
    text-align: center;
  }


</style>
