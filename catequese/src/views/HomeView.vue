<template>
  <main>
    <input type="text" placeholder="Digite seu nome" v-model="exemplo">
    <p>Essa mensagem é {{ exemplo }}</p>
    <input type="text" v-model="cadastro.nome">
    <input type="number" v-model="cadastro.idade">
    <button @click="button">Enviar</button>
  </main>
</template>

<script>
export default {
  data() {
    return {
      exemplo: null,
      cadastro: {
        nome: null,
        idade: null
      }
    }
  },
  methods: {
    button() {
      console.log('alguma coisa...')
    }
  }
}
</script>
