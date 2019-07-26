<template>

  <header id="header">
    <div class="container main-menu">
      <div class="row align-items-center justify-content-between d-flex">
        <div id="logo">
          <a href="index.html"><img src="@/assets/img/logo.png" alt="" title="" /></a>
        </div>
        <nav id="nav-menu-container">
          <ul class="nav-menu">
            <li><nuxt-link to="/" exact>Home</nuxt-link></li>
            <li><nuxt-link to="/about">About</nuxt-link></li>
            <li><nuxt-link to="/blog">Blog</nuxt-link></li>
            <li><nuxt-link to="/contact">Contact</nuxt-link></li>
          </ul>
        </nav><!-- #nav-menu-container -->
      </div>
    </div>
  </header>

</template>

<script>
    export default {
        name: "PageHeader"
    }
</script>
