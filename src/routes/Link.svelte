<script lang="ts">
  import { goto } from "$app/navigation";

  export let target: string;
  export let label: string;
</script>

<button on:click={ () => goto(target) }>{label}</button>
