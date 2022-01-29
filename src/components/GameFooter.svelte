<script>
  import Button from "./Button.svelte";
  import game from "../store/game.store";
</script>

<style>
  footer {
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    padding: 1rem 0;
    /* height: 74px; */
  }

  .credits {
    color: white;
    padding: 10px 20px;
    border-radius: 20px;
    background: -webkit-linear-gradient(top, #ff5db1 0%, #ef017c 100%);
    text-transform: uppercase;
    letter-spacing: 1px;
    text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
    border: 4px solid white;
  }

  .credits p {
    margin: 6px 0;
  }

  .credits a {
    color: #ffe1f0;
    text-decoration: underline;
  }
</style>

<footer>
  <div class="credits">
    <p>Svelte Crush by <a href="https://www.twitter.com/charca" target="_blank">@charca</a></p>
    <p>Source code on <a href="https://www.github.com/charca/svelte-match3" target="_blank">GitHub</a></p>
  </div>
  <Button on:click={game.reset}>Reset</Button>
</footer>
