<template>
  <div class="container">
    <ul>
        <li>
            <img src="../assets/img/buy-comics-digital-comics.png" alt="comics digital">
            <a href="#">DIGITAL COMICS</a>
        </li>
        <li>
            <img src="../assets/img/buy-comics-merchandise.png" alt="merch">
            <a href="#">DC MERCHANDISE</a>
        </li>
        <li>
            <img src="../assets/img/buy-comics-subscriptions.png" alt="sub">
            <a href="#">SUBSCRIPTION</a>
        </li>
        <li>
            <img src="../assets/img/buy-comics-shop-locator.png" alt="shop">
            <a href="#">COMIC SHOP LOCATOR</a>
        </li>
        <li>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="power">
            <a href="#">DC POWER VISA</a>
        </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.container {
  background-color: #007cf2;
  
}

/*****************************
               LISTA
*******************************/

ul {
  list-style-type: none;
  display: flex;
  justify-content: space-between;
  width: 80%;
  margin: auto;
  padding: 0;
  
}

li {
  display: flex;
  align-items: center;
}

li img{
  height: 50%;
}

a {
  text-decoration: none;
  color: white;
  align-items: center;
}
</style>