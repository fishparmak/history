<template>
  <div id="app">
    <Title secondary>{{ msg }}</Title>
    <Date> {{ date }} </Date>
    <ul>
      <li v-for="item in analytics">
        <analytics :post="item"></analytics>
      </li>
    </ul>
  </div>
</template>

<script>
import Title from './components/Title.vue';
import Date from './Date.vue';
import Analytics from "./components/Analytics.vue";

export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      date: 'April 2016',
      analytics: [
        {title: "20+", content: "Hours of work"}, 
        {title: "10 000+", content: "Views"}, 
        {title: "12", content: "Team members"}
      ]
    }
  },
  components: {
    Title,
    analytics: Analytics,
    Date
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
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
</style>
