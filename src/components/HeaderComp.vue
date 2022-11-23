<template>
  <div class="container">
    <div class="navbar">
      <div><img src="../assets/img/dc-logo.png" alt="logo" /></div>
      <div class="lista">
        <ul>
          <li><a href="#">CHARACTERS</a></li>
          <li><a href="#">COMICS</a></li>
          <li><a href="#">MOVIES</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">GAMES</a></li>
          <li><a href="#">COLLECTIBLES</a></li>
          <li><a href="#">VIDEOS</a></li>
          <li><a href="#">FANS</a></li>
          <li><a href="#">NEWS</a></li>
          <li><a href="#">SHOP</a></li>
        </ul>
      </div>
    </div>
    <div class="content">
      <div class="esistential_problem">
        <h2>--Content goes here--</h2>
      </div>
    </div>
  </div>
</template>
  


<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>
  
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss" >
.container {
  background-color: white;
}

.navbar {
  display: flex;
  justify-content: space-between;
  width: 80%;
  margin: auto;
}

/*****************************
               LISTA
*******************************/

.lista {
  align-self: center;
}

ul {
  list-style-type: none;
  display: flex;
}

li {
  margin: auto 10px;
}

a {
  color: black;
  text-decoration: none;
  font-weight: bold;
}

a:hover {
  color: rgb(64, 174, 211);
  border-bottom: 5px solid rgb(64, 174, 211);
  padding-bottom: 25px;
}

/********************
       CONTENT
*********************/
.content {
  background-color: #1f1f1f;
}

.esistential_problem {
  padding: 2.5% 0;
}

.esistential_problem h2 {
  color: white;
  margin: 0;
  width: 80%;
  margin: auto;
  font-size: 2rem;
}
</style>



