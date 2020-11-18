<template>
 <div class="Login">
 <div class="Login-back">
   <Header />
   <div class="name">
     <p>ログイン</p>
     <div class="form">
       <input placeholder="メールアドレス" type="email" v-model="email" />
       <input placeholder="パスワード" type="password" v-model="password"/>
       <button @click="auth">ログイン</button>
       <p><a @click="$router.push('/About')">パスワードをお忘れの方はこちら</a></p>
     </div>
   </div>
   <Footer />
 </div>
 </div>
</template>

<script>
import Header from "../components/Header";
import Footer from "../components/Footer";
export default {
  date(){
    return{
      email:"",
      password:""
    };
  },
  components:{
    Header,
    Footer
  },
  methods:{
    auth(){
      this.$store.dispatch("login",{
        email: this.email,
        password: this.password
      });
    }
  }   
};
</script>

<style scoped>
.Login{
    position: relative;
    background-image: url("../assets/namiki.jpg");
    background-size:cover;
}
.Login-back{
    z-index: 1;
    top:0;
    left:0;
    background-color: rgba(5,5,5,0.3);
}
.name {
  margin: 100px auto;
  width: 350px;
  border-radius: 5px;
  padding: 25px;
  background-color: rgba(245,245,245,0.3);
}
.name p {
  color: black;
  font-weight: bold;
  text-align: center;
}
.name a {
    cursor: pointer;
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
  margin-bottom: 15px;
}
</style>