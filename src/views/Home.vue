<template>
 <div>
   <div class="header flex">
      <div class="left">
        <img class="logo" src="../assets/logo.png" alt />
      </div>
      <div class="right flex">
       <p>新規登録</p>
       <p>ログイン</p>
      </div>
  </div>
  <nav class="nav">
    <ul>
    <li><a href=”#”>カジュアル</a></li>
    <li><a href=”#”>北欧</a></li>      
    <li><a href=”#”>アジアン</a></li>
    <li><a href=”#”>中世西洋</a></li>
    <li><a href=”#”>中華</a></li>
    <li><a href=”#”>その他</a></li>
    </ul>
  </nav>
  <div class="main">
     <div class="left-menu">
        <div class="nouki">
          <img src="../assets/nouki.jpg">
        </div>
        <div class="howtell">
          <p>お電話でのお問い合わせ</p>
          <ul class="tell felx">
            <li>tel.</li>
            <li>0120-012-345</li>
          </ul>
          <p>営業時間</p>
          <p>平日9:00～18:00</p>
          <ul class="dey felx">
            <li id="holiday">休日</li>
            <li id="holiday-day">土・日・祝日</li>
          </ul>
        </div>   
     </div>
     <div class="main-wrap flex around">
          <div class="business-cat" v-for="(data,index) in business" :key="index">
            <img :src="data.img" alt />
            <h3>{{data.title}}</h3>
            <p>{{data.description}}</p>
          </div>
      </div> 
  </div>
  <div class="footer">
    <ul class="footer-menu">
    <li><a href=”#”>特定商取引法に基づく表記</a></li>
    <li><a href=”#”>お支払い方法について</a></li>      
    <li><a href=”#”>配送方法・送料について</a></li>
    <li><a href=”#”>営業向け</a></li>
    <li><a href=”#”>お問い合わせ</a></li>
    </ul>
    <p>ルームデザインのことならお任せ！家具と雑貨の「Rooms」 Copyright © 2020 TeamRooms. All Rights Reserved.</p>          
  </div>
  
 </div>
</template>
<script>
export default {
  data(){
    return{
      business:[
        {
          img: require("../assets/Roomie.png"),
          title: "商品A",
          description:
          "商品Aの説明が入ります。商品Aの説明が入ります。商品Aの説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品B",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品C",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品D",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        },{
          img: require("../assets/Roomie.png"),
          title: "商品A",
          description:
          "商品Aの説明が入ります。商品Aの説明が入ります。商品Aの説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品B",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品C",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品D",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        },{
          img: require("../assets/Roomie.png"),
          title: "商品A",
          description:
          "商品Aの説明が入ります。商品Aの説明が入ります。商品Aの説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品B",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品C",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品D",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        },{
          img: require("../assets/Roomie.png"),
          title: "商品A",
          description:
          "商品Aの説明が入ります。商品Aの説明が入ります。商品Aの説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品B",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品C",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品D",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        },{
          img: require("../assets/Roomie.png"),
          title: "商品A",
          description:
          "商品Aの説明が入ります。商品Aの説明が入ります。商品Aの説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品B",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品C",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        }, 
        {
          img: require("../assets/Roomie.png"),
          title: "商品D",
          description:
          "商品の説明が入ります。商品の説明が入ります。商品の説明が入ります。"
        },
      ]
    }
  }
}

</script>
<style scoped>

.header {
  margin:0 20px;
  padding:10px;
}
.logo {
  width: 120px;
  height: 70px;
  cursor: pointer;
}
.right {
  align-items: center;
}
.right p {
  margin-right: 20px;
  cursor: pointer;
  color: red;
}
.flex {
  display: flex;
  justify-content: space-between;
}

/*ナビ*/
nav{
border-bottom: 1px solid #ccc;
background-image: url(../assets/wollpaper.png);
}
nav ul{
display: table;
margin: 0 auto;
padding: 0;
width: 80%;
text-align: center;
}
nav ul li{
display: table-cell;
min-width: 50px;
border-right: 1px solid #ccc;
}
nav ul li:first-child{
border-left: 1px solid #ccc;
}
nav ul li a{
display: block;
width: 100%;
padding: 10px 0;
text-decoration: none;
color:white;
border-bottom: 5px solid rgba(0,0,0,0);
}
nav ul li a:hover{
background-color:#F8E750;
border-bottom: 5px solid #00B0F0;
color: #00B0F0;
}

/* 左側メニュー*/
.main{
  display: flex;
  margin: 10px 0;
}
.left-menu{
  width: 15%;
  margin-right: 1%; /*左側で商品一覧との空白を調節*/
  background-color: #aaa;
  text-align: center;
}
.nouki{
  margin-bottom:15px;
}
.howtell{
  background-color: white;
  padding: 10px 0;
  
}
.howtell p{
  margin:5px 0;
}
.tell{
  display: flex;
  list-style: none;
  margin-bottom: 20px;
  justify-content:center; 
}
.dey{
  display: flex;
  list-style: none;
  justify-content:center; 
}
#holiday{
  color:red;
  border: 2px red solid;
}
#holiday-day{
  border:2px rgba(0,0,0,0) solid
}

/* 商品一覧 */
.main-wrap {
  text-align: center;
  width: 84%;
}

.business-cat {
  width: 21%;
  background-color: rgba(51, 51, 51, 0.5);
  padding: 20px 35px 30px;
  box-sizing: border-box;
  margin:0 5px;
  margin-bottom: 50px;
}

.business-cat h3 {
  font-size: 18px;
  font-weight: bold;
  margin-bottom: 10px;
  color: #fff;
}

.business-cat p {
  color: #fff;
}

.business-cat img {
  width: 100px;
  height: auto;
  margin: 0 auto 10px;
}

/*フッター*/
.footer-menu{
  display: flex;
  list-style: none;
  width: 100%;
  background-color: #ccc;
  justify-content:center; 
  margin-bottom: 5px;
}
.footer-menu li{
  margin: 5px;
}
.footer-menu a{
  color:white;
}
.footer p{
  text-align:center;
  margin-bottom: 5px;
}

</style>
