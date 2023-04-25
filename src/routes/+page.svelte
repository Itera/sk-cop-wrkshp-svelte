<script lang="ts" xmlns:MenuItem="http://www.w3.org/1999/html">
  import Menu from './Menu.svelte';
  import MenuItem from './MenuItem.svelte';
  import Link from './Link.svelte';
</script>

<h1>Menu</h1>
<Menu>
  <MenuItem>
    <Link target="/game" label="Start game" />
  </MenuItem>
  <MenuItem>
    <Link target="/options" label="Options" />
  </MenuItem>
  <MenuItem>
    <Link target="/best-scores" label="Best scores" />
  </MenuItem>
</Menu>
