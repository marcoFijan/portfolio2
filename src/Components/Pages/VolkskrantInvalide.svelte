<script> 
    import ProjectPage from '/src/Components/Templates/ProjectPage.svelte';
</script>

<style>
    img{
        max-width: 100%;
        border: .5px solid rgb(150, 150, 150);
        box-sizing: border-box;
    }

    /* h3{
        border-top: .5px solid rgb(150, 150, 150);
        padding-top: 2rem;
    } */
</style>

<ProjectPage
    title={'Auto in de stad'}
    projectYear={'2020'}
    projectType={'D3 en Framework'}
    targetAudience={'Schrijvers bij de Volkskrant (vanaf 22 jaar)'}
    description={'In dit project kreeg ik de opdracht om interessante bevindingen over "de auto in de stad" te visualiseren. De visualisatie moest digitaal opgeleverd worden. Er moet dus een URL beschikbaar zijn om de visualisatie in te zien. We kregen van de Volkskrant verschillende datasets van het RDW waaruit we bevindingen konden halen. Om deze data mooi online te visualiseren, gebruik ik D3. Uit die visualisatie kan de Volkskrant de interessante bevinding opnemen en hierover een artikel plaatsen. Ik hoef zelf geen artikel te schrijven. Eventueel kan ik wel wat kleine conclusies noteren in de visualisatie.'}
    githubLink={'https://github.com/marcoFijan/frontend-applications'}
    liveLink={'https://cocky-northcutt-c3cbf4.netlify.app/'}>
        <h3>Benodigde beschikbare invalide parkeerplekken</h3>
        <img src="/volkskrantInvalide.jpg" alt="Volkskrant project - Invalide parkeerplekken"/>
        <p>Ik koos voor mijn ontwerp om me te focussen op de fysiek invaliden. Ik vroeg me af of er genoeg parkeerplekken toegankelijk zijn voor lichamelijk gehandicapten. Ik nam hiervoor de invalide cijfers van het CBS en de parkeerdata van RDW. Ik deed dit, vanwege de tijd en incomplete data, vrij globaal per provincie in plaats van per stad</p>
        <p>Op deze pagina kan er gekeken worden of de provincie naar keuze voldoende parkeerplekken heeft. Dit wordt in tekstvorm uitgelegd. Met behulp van svelte wordt deze tekst automatisch aangepast met de juiste gegevens</p>
        <p>Daarna kunnen provincies met elkaar vergeleken worden. Hier wordt weergegeven hoeveel procent van de bevolking van een provincie een lichamelijke handicap heeft.</p>
        <p>Vervolgens wordt er met D3 een stapel staafdiagram getoond waar er gekeken kan worden wat de verhoudingen zijn voor toegankelijke parkeerplekken. Daarnaast kan deze diagram ook gefiltert worden.</p>
</ProjectPage>