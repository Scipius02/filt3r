
<template>
  <footer class="navbar site-footer" id="site-footer">
    <div class="container" id="footer-container">
      <ul class="nav navbar-nav" id="footer-ul">
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
/* is not properly sticking to bottom of screen when insufficient elements on page */
#site-footer{
  background: #23395d;
  position: sticky;
  bottom: 0;
  width: 100%;
}

#footer-container {
  display: flex;
  align-content: center;
  justify-content: center;
}

#footer-ul{
  display: inline-flex;
  flex-direction: row;
  align-content: center;
}

li{
  display:inline-block;
  padding-right: 2em !important;
  padding-left: 2em !important;
}
</style>