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
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQTf9d3vymakpWH5l6ZT7FHXPWmVATlApygyg&usqp=CAU" alt="Jane" style="width:100%">
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
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQYQNvPmltFHzoHEa9xWNRt1bh2G44GfJZxFw&usqp=CAU" alt="Mike" style="width:100%">
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
      <img src="data:image/jpeg;base64,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" alt="John" style="width:100%">
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