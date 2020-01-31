<template>
  <div>
    <router-view></router-view>
    <button @click="toUsers">Usersのページにいく</button>
  </div>
</template>


<script>
export default {
  methods: {
    toUsers(){
      this.$router.push({
        name: 'users-id-profile', params: { id: 1}
      })
    }
  }
}
</script>
