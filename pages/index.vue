<template>
  <container class="cont" style="background-color:red">
    <headerLogin/>
    <div class="principal">
      <div class="base">
        <h1>Login</h1>
        <input type="text" name="usuario" value="Usuario" class="inputs" id="input1">
        <input type="password" name="senha" value="Senha" class="inputs" id="input2">
        <button> Enviar </button>
      </div>
    </div>
    <footers/>
  </container>
</template>

<script>

export default {
  name: 'home',
}

</script>

<style lang="scss" scoped>
  @import '@/pages/login.scss'
</style>