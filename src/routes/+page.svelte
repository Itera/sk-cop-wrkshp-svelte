<script lang="ts">
  import { goto } from "$app/navigation"
</script>

<h1>Menu</h1>
<button on:click={ () => goto("/game") }>Start game</button>
