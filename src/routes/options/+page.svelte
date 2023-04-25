<script lang="ts">
  import Menu from '../Menu.svelte';
  import MenuItem from '../MenuItem.svelte';
  import Link from '../Link.svelte';
  import { usernameStore } from '../../stores';

  let username = '';
  let displayUsername = '';
  function setUsername() {
    usernameStore.update(() => username);
    username = '';
  }

  usernameStore.subscribe((newValue: string) => (displayUsername = newValue));
</script>

<h1>Options</h1>

<p>user name: {displayUsername}</p>
<input placeholder="new user name" bind:value={username} />
<button on:click={setUsername}>set user name</button>

<Menu>
  <MenuItem>
    <Link target="/" label="Back to menu" />
  </MenuItem>
</Menu>
