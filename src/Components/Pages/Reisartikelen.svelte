<script> 
    import ProjectPage from '/src/Components/Templates/ProjectPage.svelte';
</script>

<style>
    img{
        max-width: 100%;
        border: .5px solid rgb(150, 150, 150);
        box-sizing: border-box;
    }

    div{
        position: relative; 
        width: 100%; 
        height: 0; 
        padding-top: 56.2500%;
        padding-bottom: 48px; 
        border: .5px solid rgb(150, 150, 150);
        margin-top: 1.6em; 
        margin-bottom: 0.9em; 
        overflow: hidden;
        will-change: transform;
    }

    div iframe{
        position: absolute; 
        width: 100%; 
        height: 100%; 
        top: 0; 
        left: 0; 
        border: none; 
        padding: 0;
        margin: 0;
    }

    a{
        padding-bottom: 2rem;
    }
</style>

<ProjectPage
    title={'Herontwerp Reisartikelen'}
    projectYear={'2020'}
    projectType={'Design'}
    targetAudience={'Corona getroffen reizigers'}
    description={'In dit project moest ik een herontwerp maken voor reisartikelen.nl. Reisartikelen.nl is een website die gespecialiseerd is in allerlei soort reisartikelen. Helaas zorgde de coronamaatregelen ervoor dat hun website dit jaar niet erg relevant of nuttig meer was. Ik kreeg de oprdacht om de website te herontwerpen zodat deze beter relevant is voor de coronamaatregelen en meer omzet kan draaien.'}
    githubLink={'n.v.t.'}
    liveLink={'https://www.figma.com/proto/w6Y44DPKMD8ttJCWdfOuyt/Reisartikelen.nl-HiFi-Final?node-id=1%3A2&scaling=scale-down-width'}>
    <h3>Orgineel Ontwerp</h3>
    <img src="/Reisartikelen.nlOrgineel.jpg" alt="Reisartikelen.nl - Orgineel"/>
    <p>Ik kreeg toestemming om flink van de standaard huisstijl af te stappen. Reisartikelen was namelijk ook erg opzoek om hun funnels en conversieratio te verbeteren. Uiteraard moesten de fonts en kleuren hetzelfde blijven. Ik heb me voornamelijk gefocust op verschillende commercieël ontwerp principes zoals call to action buttons, vertrouwen creeëren, social proof en content in footer.</p>
    <h3>LoFi Ontwerp</h3>
    <img src="/Reisartikelen.nl-LoFi.jpg" alt="Reisartikelen.nl - LoFi"/>    
    <p>In het eerste herontwerp zorgde ik voor een grote banner. Ook zorgde ik ervoor dat bezoekers in de header zich kunnen inschrijven voor de nieuwsbrief. De vermelde korting stimuleert bezoekers om zich in te schrijven. Ook gebruik ik veel verkoopsslogans die toepasselijk zijn voor de website onder de banner. De footer is nu ook meer opgevuld met nuttige informatie maar houdt dit inzichtelijk.</p>
    <h3>HiFi Ontwerp</h3>
    <img src="/Reisartikelen.nl-HiFi-Final.jpg" alt="Reisartikelen.nl - HIFI"/>
    <p>Na een feedbackronde van het LoFi-ontwerp ging ik verder met het ontwerp. Ik veranderde de verkoopslogans in iets wat relevanter was voor tijdens de coronamaatregelen. De knoppen ronde ik af. Dit heeft een hogere conversie. Voor het inschrijven van de nieuwsbrief ontwierp ik een nieuwe section op de pagina zelf. In de header zette ik een kleine call to action die mensen trekt naar de nieuwsbrief sectie. </p>
    <h3>Presentatie aan opdrachtgever</h3>
    <div>
        <iframe title="Presentatie Reisartikelen.nl" src="https:&#x2F;&#x2F;www.canva.com&#x2F;design&#x2F;DAEU6uDj-Eo&#x2F;view?embed"></iframe>
    </div>
    <a href="https:&#x2F;&#x2F;www.canva.com&#x2F;design&#x2F;DAEU6uDj-Eo&#x2F;view?utm_content=DAEU6uDj-Eo&amp;utm_campaign=designshare&amp;utm_medium=embeds&amp;utm_source=link" target="_blank" rel="noopener">Presentatie Landingspage Reisartikelen.nl</a> door Marco Fijan
</ProjectPage>