<template>
   <div>
    <div class="header flex">
        <div class="left">
            <img class="logo"
                 src="../assets/logo.png"
                 alt="roomsロゴ"
                 @click="$router.push('/')" />
        </div>
        <div class="right flex">
        <p @click="$router.push('/signup')">新規登録</p>
        <p @click="$router.push('/Login')">ログイン</p>
        </div>
    </div>
  </div>
</template>

<script>
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

</style>