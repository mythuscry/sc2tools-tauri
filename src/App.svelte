<script lang="ts">
  import Extend from "./lib/extend.svelte";
  import Draw from "./lib/draw.svelte";
</script>

<main>
  <header></header>
  <div class="container">
    <div class="left">
      <Extend />
    </div>
    <div class="right">
      <Draw />
    </div>
  </div>
</main>

<style>
  .container {
    display: flex;
    height: 100vh;
    overflow: hidden;
    background-color: rgb(244, 240, 240);
  }
  .left {
    width: 264px;

    background-color: rgb(23, 22, 22);
  }

  .right {
    width: 264px;
    background-color: rgb(23, 22, 22);
  }

  @media (max-width: 800px) {
    .left {
      display: none;
    } 
  }
</style>
