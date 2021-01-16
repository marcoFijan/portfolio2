<script>
  import Home from '/src/Components/Pages/Home.svelte';

</script>

<style>
  :global(*){
    font-family: 'Roboto', sans-serif;
  }

  :global(body){
    min-height: 100vh;
    background: rgb(59,167,253);
    background: linear-gradient(164deg, rgba(59,167,253,1) 0%, rgba(72,79,238,1) 100%);
    background-attachment: fixed;
  }
</style>

<Home></Home>