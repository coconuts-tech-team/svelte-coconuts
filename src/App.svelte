<script lang="ts">
  import Header from "./lib/Header.svelte";
  import Card from "./lib/Card.svelte";
</script>

<Header />
<main>
  <Card />
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
