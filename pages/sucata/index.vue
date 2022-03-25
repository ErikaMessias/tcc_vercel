// Sucata

<template>
  <container class="cont" style="background-color:red">
    <headers/>
    <div class="principal">
      <div class="base">
        <h1>Descarte Sucata</h1>
        <input type="text" name="denominacao" value="Denominação" class="inputs" id="input1">
        <input type="text" name="codigo" value="Codigo" class="inputs" id="input2">
        <input type="text" name="quant" value="Quantidade" class="inputs" id="input3">
        <input type="text" name="descricao" value="Descricao" class="inputs" id="input4">
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
@import '@/pages/sucata/sucata.scss'
</style>