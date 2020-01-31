<template>
  <nav>
    <h2>Home</h2>
    <router-link
      to="/"
      active-class="link--actuve"
      class="link"
    >Home</router-link>
    <router-link
      to="users/1/profile"
      class="link"
    >Users</router-link>
  </nav>
</template>

<style scoped>
  .link{
    margin-right:  10px;
  }
  .link--active {
    font-size: 20px;
  }
</style>

