<template>
  <div id="app">
    <Content msg="" />
    <Header msg="Componente view "/>
    <Menu msg=""/>
    <Sidebar msg="Componente view "/>
    <Article msg="Componente view "/>
    <HelloWorld msg="Primeiro app usando VUE"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'; //componente padrão
import Header from './components/Header.vue'; //cabeçalho 
import Content from './components/Content.vue'; //conteudo da pagina 
import Menu from './components/Menu.vue'; //conteudo da pagina 
import Sidebar from './components/Sidebar.vue'; //conteudo do artigo
import Article from './components/Article.vue'; //conteudo do artigo

export default {
  name: 'App',
  components: {
    HelloWorld,
    Header, 
    Content,
    Sidebar,
    Article,
    Menu
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  border: solid 1px #cccccc;  
  width: 1500px;
  margin:0 auto;
}
</style>
