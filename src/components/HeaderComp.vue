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
      <div class="jumbotron">
        <button>CURRENT SERIES</button>
      </div>
      <div class="cards">
        <CardComp v-for="(element, index) in comics"
        :key="index"
        :singleItem="element"
        />
      </div>
      <button class="loadmore">LOAD MORE</button>
    </div>
  </div>
</template>
  


<script>

import CardComp from './CardComp.vue'

export default {
  name: "HelloWorld",
  components : {
    CardComp
  },
  props: {
    msg: String,
  },
  data() {
    return {
      comics: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
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
  text-align: center;
  margin-bottom: 25px;
}

.esistential_problem {
  padding: 2.5% 0;
}

/********************
      JUMBOTRON
*********************/

.jumbotron {
  background-image: url("../assets/img/jumbotron.jpg");
  height: 400px;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: top;
  position: relative;
}

.jumbotron > button {
  color: white;
  font-weight: bold;
  border: 2px solid #007cf2;
  background-color: #007cf2;
  padding: 10px 40px;
  position: absolute;
  left: 15%;
  bottom: -5%;
}

/********************
       CARDS
*********************/

.cards{
  display: flex;
  width: 80%;
  margin: auto;
  flex-wrap: wrap;
  padding: 50px 0;
}


.loadmore{
  color: white;
  background-color: #007cf2;
  border: 2px solid #007cf2;
  padding: 10px 40px;
  align-self: center;
  font-weight: bold;
}
</style>



