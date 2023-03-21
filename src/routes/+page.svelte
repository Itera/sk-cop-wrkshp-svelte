<script lang="ts">
  import { goto } from "$app/navigation";
</script>

<h1>Menu</h1>
<ul>
  <li><button on:click={ () => goto("/game") }>Start game</button></li>
  <li><button on:click={ () => goto("/best-scores") }>Best scores</button></li>
</ul>
