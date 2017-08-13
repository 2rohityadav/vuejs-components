<template>
  <div class="user-component">
    <header class="heading">
      <h4>{{ msg }}</h4>
      <h5>{{subject}}</h5>
    </header>

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

      <div class="">
        <header>
          update component
        </header>
      </div>


      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      subject: 'i am user component'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

h4, h5, hr{
  padding: 0;
  margin: 0;
}
.user-component{
  width: 80%;
  margin: 0 auto;
  padding: 20px 0;
  background: #f3c697;
}
.heading {
  text-align: left;
  padding: 10px 20px;
  display: block;
  background: tomato;
  color: white;
  width: 80%;
  margin: 0 auto;
  line-height: 25px;
}

.container__card{
  display: flex;
  display: -webkit-box;
  display: -moz-box;
  display: -ms-flexbox;
  display: -webkit-flex;

  -webkit-flex-flow: row wrap;
  flex-flow: row wrap;

  justify-content: space-around;

  width: 80%;
  margin: 0 auto;
  background: #eee;
}
.card {
  min-height: 250px;
  max-width: 220px;
  border: 1px solid #cdcdcd;
  border-radius: 5px;
  margin: 10px;
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

@media all and (min-width: 600px) {
  .container__card {
    flex: 1 0px;
  }
}
@media all and (min-width: 800px) {
  .container__card {
    flex: 3 0px;
  }
}
</style>
