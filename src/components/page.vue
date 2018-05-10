<template>
  <div class="container">
    <div class="top">
      <div class="logo">
        <img src="../assets/logo.png">
      </div>
      <div class="title">
        <ul>
          <li>Home</li>
          <li>Women</li>
          <li>Men</li>
          <li>Components</li>
          <li>Store Locator</li>
          <li>Contact Us</li>
          <li>Buy Me!</li>
        </ul>
      </div>
    </div>
    <div class="slidePage">
      <swiper></swiper>
    </div>
    <div class="showPage">
      <showPage></showPage>
    </div>
  </div>
</template>

<script>
import swiper from './swiper'
import showPage from './showPage'

export default {
  name: 'Page',
  components: {
    swiper,
    showPage : showPage
  }
}
   
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .top {
    display: flex;
    width: 100vw;
    height: 100px;
  }
  .top .logo {
    width: 30%;
    height: 90px;
    display: flex;
    justify-content: center;
    align-items: flex-end;
  }
  .top .title {
    flex: 1;
  }
  .top .title ul{
    list-style: none;
    display: flex;
    justify-content: flex-start;
    align-items: flex-end;
    height: 90px;
  }
  .top .title li {
    font-size: 18px;
    color: orange;
    cursor: pointer;
    margin-bottom: 10px;
    margin-left: 20px;
    padding: 10px 15px;
  }
  .top .title li:hover {
    background-color: #f60;
    color: #fff;
  }
  .top .title li:nth-child(1) {
    background-color: #f60;
    color: #fff;
  }
</style>
