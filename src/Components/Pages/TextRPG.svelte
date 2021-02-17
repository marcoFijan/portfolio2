<script> 
    import ProjectPage from '/src/Components/Templates/ProjectPage.svelte';
</script>

<style>
    img{
        max-width: 100%;
        border: .5px solid rgb(150, 150, 150);
        box-sizing: border-box;
    }
</style>

<ProjectPage
    title={'TextBased RPG'}
    projectYear={'2018-2019'}
    projectType={'Javascript begrijpen'}
    targetAudience={'n.v.t.'}
    description={'Tijdens dit project begonnen we met Javascipt. Ik had al een beetje kennis van programmeren van mijn vorige studie Informatica. Maar Javascript kende ik nog niet. Ik besloot om een simpel text-based role playing game te spelen met javascript. '}
    githubLink={'https://github.com/marcoFijan/inleidingProgrammeren'}
    liveLink={'https://marcofijan.github.io/inleidingProgrammeren/'}>
        <img src="/TextRPG.jpg" alt="Begrijpen Javascript - Textbased RPG"/>
        <p>In dit project kan er gevochten worden met zwaarden en magie. De gebruiker gaat op avontuur en komt verschillende monsters tegen. Om de beurt kan hij kiezen wat hij wilt doen: Aanvallen met zwaard, aanvallen met magie, herstellen met potion of herstellen met magie.</p>
</ProjectPage>