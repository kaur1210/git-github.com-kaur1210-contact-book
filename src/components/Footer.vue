<template>
  <div class="page-container">
    <div class="content">
      <slot></slot>
    </div>

    <footer class="bg-dark text-white py-3 text-center" role="contentinfo">
      <p class="mb-0">
        &copy; {{ new Date().getFullYear() }} Contact Book. All Rights Reserved.
      </p>
      <!-- Optional Social Links -->
      <div class="mt-2">
        <a href="#" class="text-white me-3">
          <i class="fab fa-facebook"></i>
        </a>
        <a href="#" class="text-white me-3">
          <i class="fab fa-twitter"></i>
        </a>
        <a href="#" class="text-white">
          <i class="fab fa-linkedin"></i>
        </a>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
.page-container {
  margin-top: 70px !important;
  display: flex;
  flex-direction: column;
  min-height: 100vh; /* Ensure the container fills the viewport height */
}

.content {
  flex: 1;
}

footer {
  background-color: #343a40;
  color: white;
  padding: 1rem 0.5rem;
  text-align: center;
  width: 100%;
}

footer p {
  font-size: 0.9rem;
  margin: 0;
}

footer a {
  color: white;
  transition: color 0.3s ease;
}

footer a:hover {
  color: #ffc107; /* Matches the theme */
}
</style>
