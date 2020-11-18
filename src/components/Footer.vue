<template>
    <div class="footer">
    <ul class="footer-menu">
    <li><a href=”#”>特定商取引法に基づく表記</a></li>
    <li><a href=”#”>お支払い方法について</a></li>      
    <li><a href=”#”>配送方法・送料について</a></li>
    <li><a @click="$router.push('/test')">営業向け</a></li>
    <li><a href=”#”>お問い合わせ</a></li>
    </ul>
    <p>ルームデザインのことならお任せ！家具と雑貨の「Rooms」 Copyright © 2020 TeamRooms. All Rights Reserved.</p>          
  </div>
</template>

<script>
</script>

<style scoped>
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