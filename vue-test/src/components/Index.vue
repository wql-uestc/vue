<template>
  <div class="index">
      <form>
      <label>账户</label>
      <input type="text">
      <br>
      <label>密码</label>
      <input type="password" autocomplete>
      </form>
      <router-link to="/add">
      <button>登录</button>
      </router-link>
  </div>
</template>

<script>
export default {
  name: 'index',
  data () {
    return {
      
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


</style>
