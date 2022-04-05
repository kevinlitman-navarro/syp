<script>
  import rows from "../data/sheet.csv";
  import Entry from "$components/Entry.svelte";
  import App from "./App.svelte";
</script>

{#each rows as r}
  {#if r.name != ""}
    <div class="entry">
      <Entry data={r} />
    </div>
  {/if}
{/each}

<style>
  @media only screen and (max-width: 500px) {
    body {
      max-width: 318px;
      width: 19em;
    }
  }
</style>
