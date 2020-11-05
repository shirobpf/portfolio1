<template>
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
</template>

<script>
</script>

<style scoped>
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