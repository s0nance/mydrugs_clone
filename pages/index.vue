<template>
<!DOCTYPE html>
<html>
<head>
  <title>MyDrugs</title>
  <!-- Link to the font i want to use -->
  <link
  href="https://fonts.googleapis.com/css2?family=Roboto:wght@700&display=swap"
  rel="stylesheet">
  <!-- Icons -->
  <link rel="shortcut icon" type="image/x-icon"
  href="src/logos/favicon/favicon.ico">
  <!-- Ion Icons -->
  <script type="module"
  src="https://unpkg.com/ionicons@5.1.2/dist/ionicons/ionicons.esm.js"></script>
  <script
  src="https://unpkg.com/ionicons@5.1.2/dist/ionicons/ionicons.js"></script>
</head>
<body>

  <!-- Heading Bar -->
  <div class="container">
    <div class="mainHeader">
      <div>
        <nuxt-link class="link" to="/commandes">SHOP</nuxt-link>
      </div>
      <div>
        <nuxt-link class="link" to="/faq">FAQ</nuxt-link>
      </div>
      <div>
        <img class="img" src="~/assets/logo/White Logo.png">
      </div>
      <div>
        <nuxt-link class="link" to="/safety">SAFETY</nuxt-link>
      </div>
      <div>
        <nuxt-link class="link" to="/contact">CONTACT</nuxt-link>
      </div>
    </div>
  </div>


  <!-- The Carusel
  <div class="container">
    <img id="slide" src="~/assets/logo/logo_main_page.png">
    <ion-icon name="arrow-back-outline"
    id="prevBtn" class="arrowprev" onclick="back_slide()"></ion-icon>
    <ion-icon name="arrow-forward-outline"
    id="nextBtn" class="arrownxt" onclick="foward_slide()"></ion-icon>
  </div>
  -->
  <div id="demo" class="carousel slide" data-ride="carousel">

    <!-- Indicators -->
    <ul class="carousel-indicators">
      <li data-target="#demo" data-slide-to="0" class="active"></li>
      <li data-target="#demo" data-slide-to="1"></li>
      <li data-target="#demo" data-slide-to="2"></li>
    </ul>

    <!-- The slideshow -->
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="~/assets/logo/logo_main_page.png" alt="Los Angeles">
      </div>
      <div class="carousel-item">
        <img src="~/assets/slide/Slide_Blue_Pill.jpg" alt="Chicago">
      </div>
      <div class="carousel-item">
        <img src="ny.jpg" alt="New York">
      </div>
    </div>

    <!-- Left and right controls -->
    <a class="carousel-control-prev" href="#demo" data-slide="prev">
      <span class="carousel-control-prev-icon"></span>
    </a>
    <a class="carousel-control-next" href="#demo" data-slide="next">
      <span class="carousel-control-next-icon"></span>
    </a>
  </div>

</body>
</html>
</template>

<script>

</script>

<style>

* {
  user-select: none;
  overflow-y: hidden;
  margin: 0px;
}

body {
  background-color: #0e0e0e;
}

.mainHeader {
  display: flex;
  width: 100%;
  justify-content: space-around;
  font-size: 50px;
}

.mainHeader div {
  text-align: center;
  width: 20%;
}

.link {
  color: white;
  font-family: 'Roboto';
  font-weight: bold;
  text-decoration: none;
}

.link:hover {
  color: white;
}

.img {
  width: 60px;
  position: fixed;
  left: 45%;
}

#nextBtn {
  height: 10%;
  position: absolute;
  top: 50%;
  left: 95%;
  transform: translate(-50%, -50%);
}

#prevBtn {
  height: 10%;
  position: absolute;
  top: 50%;
  left: 5%;
  transform: translate(-50%, -50%);
}

.container {
  padding-top: 20px;
  width: 80%;
  height: 45%;
  position: relative;
  margin: auto;
}

ion-icon {
  color: white;
  font-size: 50px;
}

</style>
