<script>
  import Nav from "../components/Nav.svelte";
  import Footer from "../components/Footer.svelte";

  export let segment;
</script>

<style>
  main {
    position: relative;
    max-width: 56em;
    padding: 2em;
    margin: 0 auto;
    box-sizing: border-box;
  }

  .nav__wrap {
    max-width: 56em;
    margin: 0 auto;
  }

</style>

<div class="nav__wrap">
  <Nav {segment} />
</div>

<main>
  <slot />
</main>

<div class="footer__wrap">
  <Footer />
</div>
