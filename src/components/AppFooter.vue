<template>
  <footer class="app-footer">
    <div class="footer-content">
      <div class="footer-item">
        <b-icon icon="telephone"></b-icon> (022) 2535545
        <span class="mr-3"></span>
        <b-icon icon="inbox-fill"></b-icon> mahsyari@email.com
      </div>
      <div class="footer-item">
        <strong>Follow Us and get a chance to win 80% off</strong>
      </div>

      <div class="footer-item">
        <div class="social-media-icons">
          <strong>Follow Us:</strong>
          <span class="mr-3"></span>
          <b-icon icon="telephone" href="#" target="_blank" class="mr-3"></b-icon>
          <b-icon icon="youtube" href="#" target="_blank" class="mr-3"></b-icon>
          <b-icon icon="facebook" href="#" target="_blank" class="mr-3"></b-icon>
          <b-icon icon="twitter" href="#" target="_blank"></b-icon>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
};
</script>

<style scoped>
.app-footer {
  background-color: #333;
  color: #fff;
  padding: 10px;
  text-align: center;
}

.footer-content {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}

.footer-item {
  margin-bottom: 8px;
}

.social-media-icons a {
  color: #fff;
  font-size: 18px;
}
</style>
