<script>
  import { Button } from 'sveltestrap';
  import NavBar from './lib/NavBar.svelte';
  import app from './main';

  const color = 'primary'

  let count = 0;

  function increment() {
    count += 1;
  }
</script>

<main>
  <h1>Svelte CTF</h1>
  <NavBar />
  <p>Counter = {count}</p>
  <Button {color} on:click={ increment }>Increment</Button>
</main>



