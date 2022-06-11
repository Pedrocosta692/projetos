<template>
  <div id="app">

    <BarraNavegacao />
    <PrimeiraPaginaCarrossel />

  </div>
</template>

<script>
import './styles/global.css'
import BarraNavegacao from './components/BarraNavegacao';
import PrimeiraPaginaCarrossel from './components/PrimeiraPaginaCarrossel';


export default {
  name: 'App',
  components: {
    BarraNavegacao,
    PrimeiraPaginaCarrossel
}
}
</script>
