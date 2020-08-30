<script>
  export let open = false;
</script>

<style>
  aside {
    left: -100%;
    transition: left 0.3s ease-in-out;
  }

  .open {
    left: 0;
  }
</style>

<aside class="absolute w-full h-full bg-green-200 border-r-2 shadow-lg" class:open>
  <nav class="p-12 text-xl">
    <a class="block" href="home">Home</a>
    <a class="block" href="resume">Resume</a>
    <a class="block" href="about">About</a>
  </nav>
</aside>
