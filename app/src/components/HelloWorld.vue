<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>{{ text }}</h2>
    <div style="background: red">
      <MyComponent></MyComponent>
    </div>
  </div>
</template>

<script>
import MyComponent from './MyComponent'
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  components: {
    MyComponent
  },
  data(){
    return {
      text: "Hello world from component"
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
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
</style>
