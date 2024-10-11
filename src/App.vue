<script setup>
import { ref } from 'vue';
import SectionOne from "@/components/SectionOne.vue"
import Sponsors from "@/components/Sponsors.vue"
</script>

<template>
  <main class="all">
  <div class="app">
    <div class="navbar">
      <div class="logo"><img src="@/assets/riseNav.svg" alt="Navlogo"></div>
      <div class="nav-links">
        <ul>
          <p><a href="#home">Home</a></p>
          <p><a href="#products">Products</a></p>
          <p><a href="#investments">Investment Club</a></p>
          <p><a href="#blog">Blog</a></p>
          <p><a href="#about">About Us</a></p>
          <p><a href="#faqs">FAQs</a></p>
        </ul>
      </div>
    </div>
  </div>

  <section>
    <SectionOne />
    <Sponsors/>
  </section>

  <img src="@/assets/section.svg" alt="section" class="section-lg">
  <img src="@/assets/sectionSM.svg" alt="section" class="section-sm">

  <footer class="footer">
    <div class="footer-content">
      <div class="footer-section">
        <h3><img src="@/assets/rise.svg" alt="footerLogo"></h3>
        <ul>
          <li><a href="#about">About Us</a></li>
          <li><a href="#careers">Careers</a></li>
          <li><a href="#faqs">FAQs</a></li>
          <li><a href="#contact">Contact Info</a></li>
          <li><a href="#press">Press</a></li>
          <li><a href="#home">Rise Impact</a></li>
        </ul>
      </div>
      <div class="footer-section">
        <h3>Explore</h3>
        <ul>
          <li><a href="#home">Investment Club</a></li>
          <li><a href="#about">Blog</a></li>
        </ul>
      </div>
      <div class="footer-section">
        <h3>Products</h3>
        <ul>
          <li>Rise App</li>
          <li>Wallets</li>
          <li>Asset Classes</li>
        </ul>
      </div>
      <div class="footer-section">
        <h3>Contact Us</h3>
        <div class="social-links">
          <a href="#" class="social-link">0818 714 7405</a>
          <a href="#" class="social-link">hello@rise.capital</a>
          <a href="#" class="social-link">Newsletter </a>
          <a href="#" class="social-link">Instagram</a>
          <a href="#" class="social-link">Twitter (X)</a>
        </div>
      </div>
    </div>
  </footer>
</main>
</template>

<style scoped>
.app {
  min-width: 100%;
}

.navbar {
  display: block;
}

.navbar .nav-links {
  display: none;
}

.section-lg {
  display: none;
}

.section-sm {
  display: block;
}

.footer {
  color: #333;
  min-width: 100%;
}

.footer-content {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
}

.footer-section {
  flex: 1;
  min-width: 200px;
  margin-bottom: 1rem;
}

.footer-section h3 {
  font-weight: 600;
  margin-bottom: 1rem;
}

.footer-section ul {
  list-style: none;
  padding: 0;
}

.footer-section ul li {
  margin-bottom: 0.5rem;
}

.footer-section a {
  color: #333;
  text-decoration: none;
}

.footer-section a:hover {
  text-decoration: underline;
}

.social-links {
  display: flex;
  flex-direction: column;
}

.social-link {
  margin-right: 1rem;
  margin-bottom: 0.5rem;
}


@media (min-width: 1280px) {
  .all {
    min-width: 100%;
  }

  .app {
    min-width: auto;
  }

  .navbar {
    margin-top: 10px;
    margin-left: auto;
    margin-right: auto;
    display: flex;
    flex-direction: row;
    align-items: center;
    padding: 10px;
  }

  .navbar .nav-links {
  display: block;
  justify-items: end;
}

.section-lg {
  display: block;
}

.section-sm {
  display: none;
}

  .nav-links ul {
  display: flex;
  flex-direction: row;
  gap: 1rem;
}

  .footer {
    color: #333;
    padding: 2rem 0;
    min-width: 100vh;
  }

  .footer-content {
    display: grid;
    grid-template-columns: repeat(4, minmax(0, 1fr));
  }
}
</style>
