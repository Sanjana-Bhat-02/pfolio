<script>
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
  import "./styles.css";

</script>

<body class="bg-slate-950">
  <header>
    <Header />
  </header>

  <div class="flex flex-col flex-1">
    <!-- Content -->
    <slot />
    <footer class="mt-0">
      <Footer />
    </footer>
  </div>

  
</body>

<style>
 
</style>
