<template>
    <div class="main-wrap flex around">
        <div class="business-cat" v-for="(data,index) in business" :key="index">
        <img :src="data.img" alt />
        <h3>{{data.title}}</h3>
        <p>{{data.description}}</p>
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
</style>