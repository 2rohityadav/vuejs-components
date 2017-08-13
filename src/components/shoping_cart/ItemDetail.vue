<template>
  <div class="hello">
    <h4>{{ msg }}</h4>

  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Item Details'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
a {
  color: #42b983;
}
</style>
