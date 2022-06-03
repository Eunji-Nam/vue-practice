<template>
  <h1>Hello {{ animal }}</h1>
  <h2>원숭이는 {{ food }}를 좋아합니다.</h2>
  <input type="text" v-model="food" />
  <a :href="food">{{food}}</a>
  <hr />
  <h2 v-bind:class="{ red : food==='apple' , 'not-good' : food==='rice' }">원숭이는 {{food}}를 좋아합니다. </h2>
</template>

<script>
export default {
  name: 'App',
  data() { 
    return {
      // key: "value",
      animal: "Monkey",
      food: "apple",
      imageSource: "https://placeimg.com/100/100/any",
      naverUrl: "https://www.naver.com"
    }
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
