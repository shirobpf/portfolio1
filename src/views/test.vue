<template>
  <div>
    <Header />
    <div class="login">
      <p>ログイン</p>
      <div class="form">
        <input placeholder="メールアドレス" type="email" v-model="email" />
        <input placeholder="パスワード" type="password" v-model="password" />
        <button @click="auth">ログイン</button>
        <p>{{email}}</p>
        <p>{{password}}</p>
        <p>{{$store.state.email}}</p>
        <p>{{$store.state.password}}</p>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Header";
import Footer from "../components/Footer";
export default {
  data() {
    return {
      email: "",
      password: ""
    };
  },
  components: {
    Header,
    Footer
  },
  methods: {  
    auth() {
      this.$store.dispatch("login", {
        email: this.email,
        password: this.password
      })
      ;
    }
  }
};
</script>

<style scoped>
.form input{
    display: block;
}

</style>