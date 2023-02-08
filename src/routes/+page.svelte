<script lang="ts">
  let count = 1;

  function increment(): void {
    count += 1;
  }

  function decrement(): void {
    count -= 1;
  }
</script>

<h1>Welcome to SvelteKit!</h1>
<p>The current count is {count}.</p>
<button on:click={increment}>Increment</button>
<button on:click={decrement}>Decrement</button>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
