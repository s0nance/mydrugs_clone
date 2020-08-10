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
  <div class="mainHeader">
    <nuxt-link class="Shop" to="/commandes">SHOP</nuxt-link>
    <nuxt-link to="/faq">FAQ</nuxt-link>
    <div><img class="img" src="~/assets/logo/White Logo.png"></div>
    <nuxt-link to="/safety">SAFETY</nuxt-link>
    <nuxt-link to="/contact">CONTACT</nuxt-link>
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
  <div id="carouselExampleControls" class="carousel slide" data-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="~/assets/logo/logo_main_page.png" class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="~/assets/slide/Slide_Red_Pill.jpg" class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="~/assets/slide/Slide_Blue_Pill.jpg" class="d-block w-100" alt="...">
    </div>
  </div>
  <a class="carousel-control-prev" href="#carouselExampleControls" role="button" data-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="carousel-control-next" href="#carouselExampleControls" role="button" data-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
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
  width: 100%;
  display: flex;
  justify-content: space-around;
  font-size: 50px;
}

.mainHeader div {
  text-align: center;
  width: 20%;
  font-size: 16px;
  font-size: 2.5vw;
  text-decoration: none;
  color: white;
  font-weight: bold;
  font-family: 'Roboto';
}

.mainLink {
  text-align: center;
  width: 20%;
  text-decoration: none;
  color: white;
  font-weight: bold;
  font-family: 'Roboto';
}

.Shop {
  text-align: center;
  width: 20%;
  text-decoration: none;
  color: white;
  font-weight: bold;
  font-family: 'Roboto';
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
