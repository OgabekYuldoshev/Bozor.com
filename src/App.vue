<template>
  <div id="app">
    <div class="ishvaqt">
      <p>Bozor.<span>com</span>ga Xush Kelibsiz. Ish vaqti: <span>Dush-Yak 9:00 - 17:00</span></p>
      <p><i class="fas fa-phone-alt"></i> Telfon: (+99) 830 00 01 - (+99) 830 00 02</p>
    </div>
  <Nav/>
  <Menu/>
  <Brend/>
  <ShopCard/>
  <div class="banner">
  </div>
  <NewItem/>
  <div class="server">
    <div class="service">
      <i class="fas fa-box"></i>
      <h3>Dunyo buylab yetkazish</h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae possimus.</p>
    </div>
    <div class="service">
      <i class="fas fa-box"></i>
      <h3>Dunyo buylab yetkazish</h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae possimus.</p>
    </div>
    <div class="service">
      <i class="fas fa-box"></i>
      <h3>Dunyo buylab yetkazish</h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae possimus.</p>
    </div>
    <div class="service">
      <i class="fas fa-box"></i>
      <h3>Dunyo buylab yetkazish</h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Repudiandae possimus.</p>
    </div>
  </div>
  <div class="contact">
    <ul class="phone">
      <li>
        <i class="fas fa-phone-alt"></i>
        <div>
          <span>Manzil</span>
        <p>Toshkent sh, Shota 12</p>
        </div>
      </li>
      <li>
        <i class="fas fa-phone-alt"></i>
        <div>
          <span>Email</span>
        <p>info@bozor.com</p>
        </div>
      </li>
      <li>
        <i class="fas fa-phone-alt"></i>
        <div>
          <span>Telefon</span>
        <p>(+99) 830 00 01 - (+99) 830 00 02</p>
        </div>
      </li>
    </ul>
    <div class="social">
      <hr>
      <p>
        Bizni kuzatib boring
      </p>
      <a href="#">
        <i class="fab fa-instagram"></i>
      </a>
      <a href="#">
        <i class="fab fa-telegram"></i>
      </a>
      <a href="#">
        <i class="fab fa-twitter"></i>
      </a>
      <a href="#">
        <i class="fab fa-facebook"></i>
      </a>
    </div>
  </div>
  <footer>
    <h1>LOGO</h1>
    <p> &#169; 2019 Bozor.com Barcha huquqlar himoyalangan.  </p>
  </footer>
  </div>
</template>

<script>
import Nav from "./components/Nav"
import Menu from "./components/Menu"
import Brend from "./components/Brend"
import ShopCard from "./components/ShopCard"
import NewItem from "./components/NewItem"
export default {
  name: 'App',
  components:{
    Nav,
    Menu,
    Brend,
    ShopCard,
    NewItem
  }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
ul{
  list-style: none;
}
a{
  text-decoration: none;
}
input:focus, button:focus, select{
  outline: none;
}
.ishvaqt{
  width: 100%;
  height: 40px;
  background: #040397;
  display: flex;
  padding: 0 30px;
  align-items: center;
  justify-content: space-between;
}
.ishvaqt p:nth-child(1){
  color: white;
}
.ishvaqt p:nth-child(2){
  color: white;
}
.ishvaqt p:nth-child(1) span{
  color: gold;
}
.banner{
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 10px 30px;
  background:gray ;
  background-size: cover;
  height: 25vh;
}
.server{
  background: lightgray;
  padding: 0 30px;
  height: 30vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.service{
  display: grid;
  align-items: center;
  justify-content: center;
  text-align: center;
  width: 20%;
  height: 10vh;
}
.service i{
  font-size: 5vh;
}
.service h3{
  padding: 20px 0;
}
.contact{
  width: 100%;
  padding: 0 30px;
  height: 8vh;
  background: #040397;
  display: flex;
  align-items: center;
  justify-content: space-between;
  color: white;
}
.phone{
  display: flex;
}
.phone li{
  display: flex;
  align-items: center;
  justify-content: center;
  padding-right: 40px;
}
.phone i{
  font-size: 18px;
  margin-right: 10px;
}
.phone li span{
  color: gold;
}
.social{
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.social a{
  color: #040397;
  background: white;
  width: 4vh;
  height: 4vh;
  margin-right: 20px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.social p{
  padding:  0 20px;
}
.social hr{
  height: 6vh;
  background: none;
  border-right: 1px solid lightgray;
}
footer{
  height: 15vh;
  width: 100%;
  padding: 30px 0;
  display: grid;
  align-items: center;
  justify-content: center;
  text-align: center;
}
@media only screen and (max-width:600px) {
  .ishvaqt p:nth-child(1){
    font-size: 10px;
  }
  .ishvaqt p:nth-child(2){
    display: none;
  }
}
</style>
