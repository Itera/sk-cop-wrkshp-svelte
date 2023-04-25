<script lang="ts">
  import Menu from '../Menu.svelte';
  import MenuItem from '../MenuItem.svelte';
  import Link from '../Link.svelte';
  import { usernameStore } from '../../stores';

  let username = '';

  usernameStore.subscribe((newValue) => (username = newValue));
</script>

<h1>Game</h1>

<p>Username: {username}</p>

<Menu>
  <MenuItem>
    <Link target="/" label="Back to menu" />
  </MenuItem>
</Menu>
