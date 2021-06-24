<script lang="ts">
  import Header from "./lib/Header.svelte";
  import Cards from "./lib/Cards.svelte";
  import { Container } from "sveltestrap";
  import { Styles } from "sveltestrap";
</script>

<Styles />

<Header />
<main>
  <Container>
    <Cards />
  </Container>
</main>

<style lang="scss">
  :root {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  }
  :global(body) {
    margin: 0px;
  }
</style>
