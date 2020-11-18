<template>
  <div class="SignUp">
    <Header />
        <div class="namecard">
            <p>新規登録</p>
            <div class="form">
                <input placeholder="メールアドレス" type="email" v-model="email"/>
                <input placeholder="パスワード" type="password" v-model="password"/>
                <input placeholder="お名前" type="text" v-model="name"/>
                <input placeholder="電話番号" type="text" v-model="telnumber"/>                
                <button @click="auth">新規登録</button>
            </div>
        </div>
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Header";
import Footer from "../components/Footer";
import axios from "axios";
export default {
  data(){
    return{
      email: "",
      password: "",
      name: "",
      telnumber:""
    };
  },
    components:{
        Header,
        Footer
    },
    methods:{
      auth(){
        axios
          .post("http://127.0.0.1:8000/api/register",{
            email:this.email,
            password:this.password,
            name:this.name,
            telnumber:this.telnumber
          })
          .then(response => {
            console.log(response);
            this.$router.replace("/");
          })
          .catch(error => {
            alert(error);
          });
      }
    }  
};
</script>

<style scoped>
.SignUp{
    position: relative;
    background-color:rgba(5,5,5,0.3);
    background-size:cover;
}
button {
  width: 100px;
  text-align: center;
  padding:6px 10px;
  color: #fff;
  background-color:rgb(255, 156, 25);
  border-radius: 25px;
  cursor: pointer;
}
.namecard {
  margin: 100px auto;
  width: 350px;
  background:  rgba(245,245,245,0.3);
  border-radius: 5px;
  padding: 20px;
}
.namecard p {
  color: black;
  font-weight: bold;
  text-align: center;
}
input {
  margin-top: 15px;
  width: 80%;
  border-radius: 10px;
  padding: 10px;
  border: 1px solid black;
  color: black;
}
.form {
  text-align: center;
}
.form button {
  margin-top: 15px;
}
</style>