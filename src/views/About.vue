<template>
  <div class="about-section">
  <h1>About Us </h1>
  <p>Credit score allows you to know the score on the loans you borrow.</p>
  <p>The consequences of having a low credit score.</p>
</div>

<h2 style="text-align:center">Our Team</h2>
<div class="row">
  <div class="column">
    <div class="card">
      <img src="https://www.w3schools.com/w3images/team2.jpg" alt="Jane" style="width:100%">
      <div class="container">
        <h2>Mike Ross</h2>
        <p class="title">CEO & Founder</p>
        <p>Mike a visionary leader who started credit score in 2010.</p>
        <p>mike@example.com</p>
        <p><button class="button">Contact</button></p>
      </div>
    </div>
  </div>

  <div class="column">
    <div class="card">
      <img src="https://www.w3schools.com/w3images/team1.jpg" alt="Mike" style="width:100%">
      <div class="container">
        <h2>Jane Doe</h2>
        <p class="title">Art Director</p>
        <p>Jane is a creative and her brains always see a chance to create and recreate.</p>
        <p>jane@example.com</p>
        <p><button class="button">Contact</button></p>
      </div>
    </div>
  </div>
  
  <div class="column">
    <div class="card">
      <img src="https://www.w3schools.com/w3images/team3.jpg" alt="John" style="width:100%">
      <div class="container">
        <h2>John Doe</h2>
        <p class="title">Designer</p>
        <p>John is able to  communicate a client's story, brand and ideas to the company and put it to work.</p>
        <p>john@example.com</p>
        <p><button class="button">Contact</button></p>
      </div>
    </div>
  </div>
</div>
</template>
<style lang="scss" scoped>
 .column {
  float: left;
  width: 33.3%;
  margin-bottom: 16px;
  padding: 0 8px;
}

.card {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  margin: 8px;
}

.about-section {
  padding: 50px;
  text-align: center;
  background-color: #474e5d;
  color: white;
}

.container {
  padding: 0 16px;
}
h1 {
  color: #d88d00
}

.container::after, .row::after {
  content: "";
  clear: both;
  display: table;
}

.title {
  color: #d88d00;
}

.button {
  border: none;
  outline: 0;
  display: inline-block;
  padding: 8px;
  color: white;
  background-color: #000;
  text-align: center;
  cursor: pointer;
  width: 100%;
}

.button:hover {
  background-color: #555;
}

@media screen and (max-width: 650px) {
  .column {
    width: 100%;
    display: block;
  }
}
</style>