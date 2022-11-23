<template>
  <div class="Utilities">
    <div class="linkspace">
      <div>
        <div>
          <ul>
            <li><h2>DC COMICS</h2></li>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Videos</a></li>
            <li><a href="#">News</a></li>
          </ul>
          <ul>
            <li><h2>SHOPE</h2></li>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div>
          <ul>
            <li><h2>DC</h2></li>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy policy (New)</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscription</a></li>
            <li><a href="#">Talent Workshop</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratinggs</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>
          </ul>
        </div>
        <div>
          <ul>
            <li><h2>SITES</h2></li>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
          </ul>
        </div>
      </div>
      <!--immagine logo -->
      <div>
        <img src="../assets/img/dc-logo-bg.png" alt="favicon"/>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.Utilities {
  background-image: url('../assets/img/footer-bg.jpg');
}

/*******************
      LISTA
*******************/

ul {
  list-style-type: none;
}

li {
  color: white;
}

a {
  color: rgb(179, 176, 176);
  text-decoration: none;
}

.linkspace {
  width: 80%;
  margin: auto;
  display: flex;
  justify-content: space-between;
}

.linkspace > div{
  display: flex;
}
</style>