<template>
  <div class="LeftMenu">
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
</template>

<script>

</script>

<style scoped>
/* 左側メニュー*/
.LeftMenu{
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
</style>