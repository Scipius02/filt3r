<template>
  <footer class="navbar site-footer">
    <div class="container">
      <ul class="nav navbar-nav">
        <li class="nav-item nav-link">Contact</li>
        <li class="nav-item nav-link">Blog</li>
        <li class="nav-item nav-link">About</li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
  name: "SiteFooter"
};
</script>

<style>
.navbar{
  background:#5DBAE8;
}
.site-footer{
  background:#23395d;
}

.site-footer li{
  display:inline;
  /*align-items:center;*/
}
</style>