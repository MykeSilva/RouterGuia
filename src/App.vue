/*                    Aula 288 Router Link 17/05/23 00:00 */

<template>
  <div id="app">
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
<!--(1-288) EU QUERO APONTAR ESSE LINK PARA A ROTA /VICTOR, INSERINDO OS DOIS PONTOS : E O TRANSFORMO EM LINKS
(2-289) ESTÁTICOS-->  <!--VOU UTILIZAR O NOME DA ROTA, "VICTOR"-->
      <router-link :to="{name: 'Victor',params: {dado:'Lima1'}}">Saiba mais sobre Victor</router-link>
    </nav>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
