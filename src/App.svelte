<script>
  import { Styles } from 'sveltestrap';
  import NavBar from './lib/NavBar.svelte';

  let count = 0;

  function increment() {
    count += 1;
  }
</script>
<head>
  <link
    rel="stylesheet"
    href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css"/>
</head>

<main>
  <h1>Svelte CTF</h1>
  <NavBar />
  <p>Counter = {count}</p>
  <button on:click={ increment }>Increment</button>
</main>

<style>
 
</style>
