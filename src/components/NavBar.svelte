<script>
  import Logo from './Logo.svelte';
  import Hamburger from './Hamburger.svelte';
  import Menu from './Menu.svelte';

  export let sidebar = false;
</script>

<header class="flex justify-between bg-green-200 p-2 items-center text-green-600 border-b-2">
  <nav class="flex">
    <Hamburger bind:open={sidebar} />
    <Logo />
  </nav>

  <Menu />
</header>
