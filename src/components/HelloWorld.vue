<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
  <h2>Meu primeiro projeto Vue </h2>
  <h2>Utilize o contador: {{ counter }}</h2>
  <button id="soma" @click="somar">Somar :)</button>
  <button id="sub" @click="subtrair">Subtrair</button>
  <button id="add10" @click="verTime">Adicionar mais 10</button>
  <h1 id="titulo">Rafael dRS VueJs/VueEx</h1>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: () => ({
    counter: 0
  }),
  methods: {
    //" Chamando os métodos dos buttons"
    verTime: function() {
      this.counter = this.counter + 10
    },
    subtrair: function() {
      this.counter--
    },
    
    somar: function() {
      this.counter++
    }
  } ,
  props: {
    msg: String
  } 

}
</script>

<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
#titulo {
  color: darkmagenta;
}

#add10 {
  border-radius: 10%;
  border-color: palegoldenrod;
  border-left-width: 5px;
  border-right-width: 5px;
  color: black;
}

#sub {
  border-radius: 10%;
  border-right-width: 5px;
  border-left-width: 5px;
  border-color: palegoldenrod;
}

#soma {
  border-radius: 10%;
  border-color: palegoldenrod;
}

</style>

    <!--<p>
      For a guide and recipes on how to configure / customize this project,<br>
      check out the
      <a href="https://cli.vuejs.org" target="_blank" rel="noopener">vue-cli documentation</a>.
    </p>
    <h3>Installed CLI Plugins</h3>
    <ul>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel" target="_blank" rel="noopener">babel</a></li>
      <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint" target="_blank" rel="noopener">eslint</a></li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">Forum</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">Community Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">Twitter</a></li>
      <li><a href="https://news.vuejs.org" target="_blank" rel="noopener">News</a></li>
    </ul>
    <h3>Ecosystem</h3>
    <ul>
      <li><a href="https://router.vuejs.org" target="_blank" rel="noopener">vue-router</a></li>
      <li><a href="https://vuex.vuejs.org" target="_blank" rel="noopener">vuex</a></li>
      <li><a href="https://github.com/vuejs/vue-devtools#vue-devtools" target="_blank" rel="noopener">vue-devtools</a></li>
      <li><a href="https://vue-loader.vuejs.org" target="_blank" rel="noopener">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">awesome-vue</a></li>
    </ul>
  </div>
</template>


<-- Add "scoped" attribute to limit CSS to this component only --

-->