<script>
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
  import "./styles.css";
</script>

<div class="flex flex-col min-h-screen bg-slate-950 bg-cover">
  <header class="sticky top-0 z-50">
    <Header />
  </header>

  <div class="flex-grow">
    <div class="overflow-y-auto">
      <!-- Content -->
      <slot />
    </div>
  </div>

  <footer class="fixed z-7">
    <Footer />
  </footer>
</div>

<style>
  header {
    inset: 0 0 auto;
  }

  footer {
    inset: auto 0 0;
  }
</style>