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

  <footer class="flex-shrink-0">
    <Footer />
  </footer>
</div>
