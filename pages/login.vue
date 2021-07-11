<template lang="pug">
  #login
    .form-wrapper
      input(type="text")
      input(type="password")
      button(@click="login") 홈으로
      button(@click="test") api test
</template>

<script>
export default {
  methods: {
    login () {
      this.$router.push('/')
    },
    async test () {
      const result = await this.$axios.$get('/api/book')
      console.log(result)
    }
  }
}
</script>

<style scoped>

</style>
