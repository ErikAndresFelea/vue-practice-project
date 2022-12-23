<template>
    <footer>
        <p>Copyright &copy; 2021</p>
        <router-link v-show="homePage" to="/about">About</router-link>
    </footer>
</template>

<script>
export default {
    computed: {
    homePage() {
      if(this.$route.path === '/') 
        return true
      else
        return false
    }
  }
}
</script>

<style scoped>
a {
    color: #333;
}

footer {
    margin-top: 30px;
    text-align: center;
}
</style>