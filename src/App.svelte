<script lang="ts">
  import Extend from "./lib/extend.svelte";
  import Draw from "./lib/draw.svelte";
  import Toolbar from "./lib/toolbar.svelte";
</script>

<main>
  <header></header>
  <div class="container">
    <div class="left-section">
      <Extend />
    </div>
    <div class="middle-section">
      <Draw />
    </div>
    <div class="right-section">
      <Toolbar />
    </div>
  </div>
</main>

<style>
  .container {
    display: flex;
    width: 100%;
    height: 100vh;
    overflow: hidden;
    background-color: rgb(244, 240, 240);
  }
  .left-section {
    width: 17%;
    background-color: rgb(23, 22, 22);
    overflow: hidden;
  }
  .middle-section {
    width: 66%;
    background-color: greenyellow;
  }
  .right-section {
    width: 17%;
    background-color: rgb(23, 22, 22);
    overflow: hidden;
  }

  @media (max-width: 1000px) {
    .left-section  {
      display: none;
    }
    .middle-section {
     flex: 1;
    }

  @media (max-width: 800px) {
    .left-section ,.right-section {
      display: none;
    }
    .middle-section {
      flex: 1;
    }
  }
  }
</style>
