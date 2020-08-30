<script>
  import NavBar from '../components/NavBar.svelte';
  import Sidebar from '../components/Sidebar.svelte';
  let open = false;
</script>

<style>
  :global(body) {
    padding: 0;
  }
</style>

<Sidebar bind:open />
<NavBar bind:sidebar={open} />

<main>
  <slot />
</main>

<svelte:head>
  <link href="https://unpkg.com/tailwindcss@^1.0/dist/tailwind.min.css" rel="stylesheet" />
</svelte:head>
