<script>
  import Home from '/src/Components/Pages/Home.svelte';

</script>

<style>
  :global(*){
    font-family: 'Montserrat', sans-serif;
    scroll-behavior: smooth; 
  }

  :global(h1){
    font-family: 'Archivo Black', sans-serif;
  }

  :global(body){
    min-height: 100vh;
    background: rgb(59,167,253);
    background: linear-gradient(164deg, rgba(59,167,253,1) 0%, rgba(72,79,238,1) 100%);
    background-attachment: fixed;
    margin:0;
  }

  @media only screen and (max-width: 900px) {
      :global(h1){
        font-size: 2.5rem !important;
      }

      :global(article){
        padding-right: 1rem !important;
        padding-left: 1rem !important;
      }
}
</style>

<Home></Home>