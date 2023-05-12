<script>
  import Background from "../components/Background.svelte";
  import Header from "../components/Header.svelte";
  import Footer from "../components/Footer.svelte";
</script>

<Background>
  <Header />
  <div class="some">
    <slot />
  </div>

<Footer />
</Background>

<style>
  .some {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 2;
  }
</style>
