<script>
  import router from 'page';

  // Pages
  import Home from '/src/Components/Pages/Home.svelte';
  import RingRing from '/src/Components/Pages/RingRing.svelte';
  import VolkskrantInvalide from '/src/Components/Pages/VolkskrantInvalide.svelte';
  import Vakantielijst from '/src/Components/Pages/Vakantielijst.svelte';
  import TextRPG from '/src/Components/Pages/TextRPG.svelte';
  import Reisartikelen from '/src/Components/Pages/Reisartikelen.svelte';
  import NotFound from '/src/Components/Pages/NotFound.svelte';
  import StandaardAanbouw from './Components/Pages/StandaardAanbouw.svelte';

  // Variables
  let page;
  let params;

  // Routes
  router('/', () => (page = Home));
  router('/StandaardAanbouw', () => (page = StandaardAanbouw));
  router('/RingRing', () => (page = RingRing));
  router('/Volkskrant-Invalide-Parkeerplaatsen', () => (page = VolkskrantInvalide));
  router('/Studentenreis-Vakantielijst', () => (page = Vakantielijst));
  router('/Simple-Textbased-RPG', () => (page = TextRPG));
  router('/Reisartikelen', () => (page = Reisartikelen));
  router('/*', () => (page = NotFound));

  router.start();

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
    background: #3ba7fd;
    background: linear-gradient(164deg, rgba(59,167,253,1) 0%, #484fee 100%);
    background-attachment: fixed;
    margin:0;
  }

  /* Scrollbar styling */
  :global(body::-webkit-scrollbar) {
      width: 9px; 
  }

  :global(body::-webkit-scrollbar-track) {
      background: #f1f1f1;
  }

  :global(body::-webkit-scrollbar-thumb) {
    background: rgb(59,167,253);
      background: linear-gradient(164deg, rgba(59,167,253,1) 0%, rgba(72,79,238,1) 100%);
      border: 2px solid #f1f1f1;
      border-radius: 2rem;
      margin: 1px;
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

<svelte:component this={page} />