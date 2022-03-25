<template>
  <div class="cont" style="background-color:red">
    <headerLogin/>
      <div class="principal">
        <div class="base">
          <h1>Login</h1>
          <form action="" >
            <input type="text" name="usuario" v-model="login.username" class="inputs" id="input1" required >
            <input type="password" name="senha" v-model="login.password" class="inputs" id="input2">
            <button type="button" v-on:click="sendLogin()"> Enviar </button>
          </form>
        </div>
      </div>
    <footers/>
  </div>
</template>

<script>

export default {
  name: 'home',
    data() {
      return {
        login: {
          username: '',
          password: ''
        }
      }
    },

methods: {
    
    sendLogin: async function() {
          this.$auth
            .loginWith("local", { data: this.login })
            .then(() => {
              
              console.log("DEU CERTO O LOGIN");
            })
            .catch((erro) => {
              this.login.username = null;
              this.login.password = null;
              console.log("erro");
              console.log(erro);
            });
    }
  }
}

</script>


<style lang="scss" scoped>
  @import '@/pages/login.scss'
</style>