<template lang="pug">
  #gnb
    .title 해축v2
    .menu-wrapper
      .menu-item
        nuxt-link(to="/") HOME
      .menu-item
        nuxt-link(to="/standing") 순위
    .profile 관리자
</template>

<script>
export default {
  name: 'GlobalNavigationBar'
}
</script>

<style scoped>
#gnb {
  display: flex;
  background-image: linear-gradient(to right, #051937, #004d7a, #008793, #00bf72, #a8eb12);
  color: white;
}
#gnb .menu-wrapper {
  display: flex;
}
</style>
