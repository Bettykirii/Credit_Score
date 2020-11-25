<template>
<div class="home">
  <section class="hero is-dark">
    <div class="hero-body">
      <div class="container">
        <h1 class="title">
          Welcome to the financial literacy portal         
        </h1>
        <h2 class="subtitle">
          Your financial literacy includes knowing  your CreditScore
        </h2>
  <div class="top-left">
      <button class="btn">Check your scores</button>

  </div>

      </div>
    </div>
  </section>
</div>
</template>
<script>
export default {
  name: 'home',
 
}
</script>
<style lang="scss" scoped>
  .hero {    
    text-align: center;
    background-image: url('https://www.transunion.com/resources/transunion/img/consumer/blog/my-credit-score-dropped-no-changes-on-my-report-D-100819.jpg');
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    height: 400px;
  }
  .hero-body .title {
    text-shadow: 4px 4px 4px rgba(0, 0, 0, 0.6);
    padding: 40px 0 20px 0;
    font-size: 60px;
  }
  .subtitle {
    text-shadow: 4px 4px 4px rgba(0, 0, 0, 0.7);
    font-size: 30px;
  }
  
    .welcome {
      width: 400px;
      padding: 10px;
      margin-left: auto;
      margin-right: auto;
    }
  
  .is-xl {
    font-size: 1.7rem;
  }
 .top-left {
  position: absolute;
  top: 8px;
  left: 16px;
}
.btn {
  background-color: green;
  color: white;
  font-size: 16px;
  padding: 12px 24px;
  border: none;
  cursor: pointer;
  border-radius: 5px;
  text-align: center;
}

.btn:hover {
  background-color: green;
}

</style>