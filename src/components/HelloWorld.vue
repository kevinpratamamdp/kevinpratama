<template>
  <div class="hello">
    <div class="topnav">
      <a class="active" href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#about">New Car</a>
      <a href="#about">Used Car</a>
      <a href="#contact">Contact</a>
      <div class="search-container">
        <form action="/action_page.php">
          <input type="text" placeholder="Search Car" name="search">
          <button type="submit">Go</button>
        </form>
      </div>
    </div>
    <h1>{{ msg }}</h1>
    <h3>Japan Cars</h3>
    <ul>
      <li><img src="https://awsimages.detik.net.id/community/media/visual/2020/03/22/e5590047-cc1c-4e33-b608-1752f46d5274_169.jpeg"></li>
      <li><img src="https://t1-client.toyota-europe.com/images/toyota-logo.jpg"></li>
      <li><img src="https://logosvector.net/wp-content/uploads/2014/10/honda-logo-vector-download.jpg"></li>
     
    </ul>
    <h3>Italy Cars</h3>
    <ul>
      <li><img src="https://seeklogo.net/wp-content/uploads/2017/01/ferrari-logo.png"></li>
      <li><img src="https://audimediacenter-a.akamaihd.net/system/production/media/28404/images/55eb0a5e2c5789e25ea1ff3ff521b414c3b70415/A160057_full.jpg?1582245524"></li>
    </ul>
    <h3>Germany Cars</h3>
    <ul>
      <li><img src="https://luxe.tv/wp-content/uploads/2020/03/Logo-Audi-1.jpg"></li>
      <li><img src="https://brandlogos.net/wp-content/uploads/2020/03/new-bmw-logo-2020-512x512.png"></li>
    </ul>
    <h3>American Cars</h3>
    <ul>
      <li><img src="https://cdn.dribbble.com/users/469697/screenshots/6449432/ford_white_4x.jpg"></li>
    </ul>
    <div class="botnav">
      <p>Collection Cars</p>
      <p>Copyright 2020 | Hosting poweres by CloudFlare</p>
      <p>Email</p>
      <p>collectioncars@gmail.com</p>
      <p>082177979924</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 100px 0 0;
  font-size: 35px;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 50px 10px;
}
a {
  color: #42b983;
}
img{
  width: 250px;
  height: 160px;
}
</style>
