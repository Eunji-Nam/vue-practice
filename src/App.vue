<template>
<div>
  <h2 v-if="display"> (if)보입니다!! </h2>
  <h2 v-show="display"> (show)보입니다!! </h2>
</div>
</template>

<script>
export default {
  name: 'App',
  data() { 
    return {
      age: 10,
      display: false
    };
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
input {
  font-size: 20px;
}

.orange {
  color: orange;
}
.salmon {
  color: salmon;
}
.red {
  color: red;
}
.not-good {
  text-decoration: line-through;
}
</style>
