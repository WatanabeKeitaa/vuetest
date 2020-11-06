<template>
  <div class="hello">
    <!-- ヘッダの呼び出し部分を作る　から -->
    <p v-if="msg.length > 0">
        {{msg}}
    </p>
    <p v-else>
        no text
    </p>
    <input type="text" v-model="msg">
    <button @click="clear()">clear</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'メッセージ、データバインディングらしい'
    }
  },
  methods: {
      clear() {
          this.msg = ''
      }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
</style>
