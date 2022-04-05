<script>
  import Header from "$components/Header.svelte";
  import Table from "$components/Table.svelte";
  import WIP from "$components/helpers/WIP.svelte";
  // import Footer from "$components/Footer.svelte";
</script>

<!-- <WIP /> -->
<div class="container">
  <Table />
</div>

<!-- <Footer /> -->
<style>
  .container {
    width: 85%;
    max-width: 880px;
    padding: 1rem;
    margin: 0 auto;
    background-color: black;
    color: #ffffff;
  }

  :global(.container) {
    margin: 2em auto;
    padding-top: 4em;
  }

  :global(.container h2) {
    font-weight: bold;
  }

  :global(.container h2 span) {
    background: var(--color-highlight);
    padding: 0 0.5em;
  }
</style>
