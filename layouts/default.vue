<template>
  <div>
    <header class="title">
        <nuxt-link class="logo" to="/">NuxtShoppingMaverick</nuxt-link>
    </header>
    <Nuxt/>
  </div>

</template>



<style scoped>
/* 헤더관련 스타일 */
header {
  height: 60px;
  display: flex;
  align-items: center;
  padding: 0 0.5rem;
}
.logo {
  font-weight: 900;
}
.logo:visited {
  color: inherit;
}
</style>