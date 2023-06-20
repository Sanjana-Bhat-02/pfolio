<script>
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
  import "./styles.css";
</script>

<body class="bg-slate-950 flex flex-col flex-1">
  <header>
    <Header />
  </header>

  <main>
    <slot />
  </main>
  
  <footer class="lg:mt-40">
    <Footer />
  </footer>
</body>

<style>
  body {
    opacity: 0;
    animation: fade-in 1s ease-in forwards;
  }

  @keyframes fade-in {
    from {
      opacity: 0;
    }
    to {
      opacity: 1;
    }
  }

  main {
  height: 100%;
  width: 100%;
}
</style>
