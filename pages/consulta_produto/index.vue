// Consulta Produto

<template>
  <container class="cont" style="background-color:red">
    <headers/>
    <div class="principal">
      <div class="base">
        <h1>Consulta de Disponibilidade</h1>
        <div class="centro">
          <input type="text" name="search" value="Nome do Produto" class="inputs" id="input1">        
          <button> Buscar </button>
        </div>
        <input type="text" name="searchs" value="" class="inputs" id="input2">
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
  @import '@/pages/consulta_produto/consulta_produto.scss'
</style>