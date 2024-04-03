<script lang="ts">
  import Greet from './lib/Map.svelte'
  import Draw from './lib/draw.svelte';
  import Extend from './lib/extend.svelte';
</script>

<main class="container">
  <div class="row" style="display: flex">
    <Extend/>
    <Greet />
    <Draw/>
  </div>

</main>

<style>

</style>