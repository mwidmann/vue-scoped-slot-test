<template>
  <the-wrapper>
    <div slot-scope="{ val, mutate }">
      <div>{{ val }}</div>
      <div><button type="button" @click="mutate">+1 💫</button></div>
      <slot></slot>
    </div>
  </the-wrapper>
</template>

<script>
import Wrapper from "./Wrapper";
export default {
  name: "HelloWorld",
  components: {
    TheWrapper: Wrapper
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
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
