<template>
<div class="home">
  <section class="hero is-dark">
    <div class="hero-body">
      <div class="banner container">
        <h1 class="title">
          Welcome to Virtual Bank       
        </h1>
        <h2 class="subtitle">
          Make sure you check out our upcoming events below
        </h2>
        <div class="button-block">
          <button class="button is-xl is-dark">Sign Up to Browse Events</button>
        </div>
      </div>
    </div>
  </section>
  <EventsList />
</div>
</template>

<script>
import EventsList from '../components/EventsList';
export default {
  name: 'home',
  components: {
    EventsList
  }
}
</script>

<style lang="scss" scoped>

  .tb1{
    border:1px solid red;
  }
  .tb2{
    border:1px solid blue;
  }
  .hero {  
    text-align: left;
    background-color: #6A95A8;
    background-image: url('/images/bank-hero.jpg');
    // background-size: cover;
    background-position: right;
    background-repeat: no-repeat;
    height: 550px;
  }
  .banner{
    float:left;
    width:700px;
    padding-left:20px;
  }
  .hero-body .title {
    text-shadow: 4px 4px 4px rgba(65, 45, 45, 0.6);
    padding: 40px 0 20px 0;
    font-size: 60px;
  }
  .subtitle {
    text-shadow: 4px 4px 4px rgba(0, 0, 0, 0.7);
    font-size: 30px;
  }
  .button-block {
    text-align: center;
    margin-left: auto;
    margin-right: auto;
    width: 100%;
    position: absolute;
    .button {
      margin-right: 50px;
      padding-left: 50px;
      padding-right: 50px;
    }
    .welcome {
      width: 400px;
      padding: 10px;
      margin-left: auto;
      margin-right: auto;
    }
  }
  .is-xl {
    font-size: 1.7rem;
  }
</style>