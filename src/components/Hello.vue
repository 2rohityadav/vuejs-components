<template>
  <div class="hello">
    <h4>{{ msg }}</h4>
    <div class="container__card">
      <div class="card">
        <header class="card__header">
          <span class="card__header-content">My Card</span>
        </header>

        <div class="card__content">
          <h3 class="card__content-heading">"My Heading"</h3>
          <img  class="card__content-image" src="http://via.placeholder.com/150x150">
        </div>

        <footer class="card__footer">
          <div class="card__footer-content">
            <span class="card__footer-item">Items</span>
            <span class="card__footer-item-count">1234</span>
          </div>
        </footer>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container__card{
  display: flex;
  width: 80%;
  margin: 0 auto;
  background: #eee;
}
.card {
  min-height: 250px;
  max-width: 220px;
  border: 1px solid #cdcdcd;
  border-radius: 5px
}

.card__header {
  padding: .5rem 1rem;
}

.card__header-content {
  display: block;
  line-height: 30px;
  text-align: center;
  border-bottom: 1px solid #cdcdcd;
  color: darkblue
}

.card__content {
  padding: .5rem 1rem 1rem;
}

.card__content-heading {
  margin: 0;
  margin-bottom: .5rem;
  font-size: .8rem;
  font-weight: normal;
  color: #999999;
  text-align: center;
}

.card__content-image {
  display: block;
  max-width: 100%;
  margin: 0 auto;
}

.card__footer {
  display: flex;
  padding: .5rem 1rem;
  border-top: 1px solid #cdcdcd;
}

.card__footer-content {
  line-height: 30px;
}

.card__footer-item {
  font-weight: bold;
  margin-right: 80px;
}

.card__footer-item-count {
  color: darkblue;
}

a {
  color: #42b983;
}
</style>
