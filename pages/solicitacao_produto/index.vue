// Solicitação de Produtos

<template>
  <container class="cont" style="background-color:red">
    <headers/>
    <div class="principal">
      <div class="base">
        <h1>Solicitação de Produtos</h1>
        <div class="centro">
        <section class="img">
            <img src="/logo.png">
        </section>

        <section class="campos">
            <input type="text" name="material" value="Material" class="inputs" id="input1">
            <input type="text" name="quant" value="Quantidade" class="inputs" id="input2">
            <input type="text" name="recebedor" value="Recebedor" class="inputs" id="input3">
        </section>
        </div>
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
@import '@/pages/solicitacao_produto/solicitacao_produto.scss'
</style>