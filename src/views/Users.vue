<template>
  <div>
    <router-link to="/users/1">ユーザー１</router-link>
    <router-link to="/users/2">ユーザー2</router-link>
    <hr>
    <div>User No. {{ id }}</div>
    <router-link :to="'/users/' + (Number(id) + 1) + '/profile'">次へ</router-link>
    <router-link :to="{ name: 'users-id-profile', params: { id: Number(id) + 1}}">次へ</router-link>
    <router-view></router-view>
  </div>
</template>


<script>
export default {
  props: ["id"]
}
</script>
