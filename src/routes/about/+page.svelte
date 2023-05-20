<script>
    import Background from "../../components/Background.svelte";
    import Header from "../../components/Header.svelte";
    import Footer from "../../components/Footer.svelte";
    import "../styles.css";
   
  </script>
  
  <div class="bg-slate-950 min-h-screen flex flex-col bg-fixed">
    <header class="sticky top-0 z-50">
      <Header />
    </header>
    <div class="overflow-y-auto">
    <Background>
      <!-- <slot/> -->
      <footer class="sticky bottom-0 z-50">
        <Footer />
      </footer>
    </Background>
    
  </div>
    
  </div>
  