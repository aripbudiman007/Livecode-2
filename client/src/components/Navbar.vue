<template>
  <nav>
      <div class="nav-left">
        <img
          src="https://mustopa28121992.github.io/projectt/img/fox--md5--a9e377ae39495073d0e66db163fc8d9b.png"
          alt="logo"
        />
        <h1>Animal Lover</h1>
      </div>
      <div class="nav-center">
        <a href="/favourites">My Favorites</a>
      </div>
      <div class="nav-right" v-if="isLogin">
        <button @click="$store.dispatch('logout')">Logout</button>
      </div>
    </nav>
</template>

<script>
export default {
  name: 'Navbar',
  data () {
    return {
      isLogin: true
    }
  }
}
</script>
