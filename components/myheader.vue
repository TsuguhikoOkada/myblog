<template>
    <div class="mb-2">
      <b-navbar toggleable="lg" type="dark" variant="dark">
        <b-navbar-brand :href="baseUrl">ブログ</b-navbar-brand>
        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-navbar-nav>
          <b-nav-item :href="baseUrl + 'profile'">プロフィール</b-nav-item>
        </b-navbar-nav>
      </b-navbar>
    </div>
  </template>
  
  <script>
  export default {
    computed: {
      baseUrl() {
        return this.$router.options.base;
      }
    }
  }
  </script>
  