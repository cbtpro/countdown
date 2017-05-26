<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
import utils from './utils'
export default {
  name: 'hello',
  data () {
    return {
      msg: [
        '你的人生还剩下许多，遇到挫折不要气馁。接下来的日子，你要继续努力！',
        '你的人生已经所剩无几了，回想走过的日子，是不是还有些许遗憾？趁着还没有谢幕，让人生不留遗憾吧。',
        '你还很年轻，人生的路才刚刚开始，趁着青春年少，做自己梦想的事吧！',
        '你的人生走完了一半，如果你激情还尚存，不要让懒惰磨灭了他们！'
      ][utils.getRandomInt(0, 3)]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
