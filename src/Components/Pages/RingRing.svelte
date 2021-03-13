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
    title={'Ring Ring Dashboard'}
    projectYear={'2021'}
    projectType={'Design en Datavisualisatie'}
    targetAudience={'Beleidsmakers Ring Ring (35-70 jaar)'}
    description={'Tijdens dit project kreeg ik de opdracht van Ring Ring om een dashboard te ontwerpen voor de beleidsmakers. Ring Ring is een bedrijf dat met haar app data verzameld over fietsverkeer en probeert met haar app mensen te motiveren om meer te fietsen. Daarnaast wilt Ring Ring ook graag feedback ontvangen en visualiseren over haar gebruikers en hun fietsroutes. Voor het dashbaord kregen we een geojson met onder andere de coordinaten van de routes, de snelheid, de start en einddatum en tijd, de feedback met feedbackscore en de afgelegde afstand'}
    githubLink={'https://github.com/marcoFijan/projectDatavisualisation'}
    liveLink={'https://marcofijan.github.io/projectDatavisualisation/'}>
     <h3>Inlogpagina</h3>
        <img src="/RingRing1.jpg" alt="Ring-Ring SignIn"/>
        <p>Aangezien dit dashboard privé RingRing data bevat, is er een inlogpagina waar er ingelogd dient te worden.</p>
        <h3>Dashboard</h3>
        <img src="/RingRing2.jpg" alt="Ring-Ring Dashboard"/>
        <p>Op de dashboardpagina wordt er een globaal overzicht getoond waar alle deatilpagina's zichbaar zijn: Kaart, datavisualisatie en feedback</p>
        <h3>Voor u pagina</h3>
        <img src="/RingRing3.jpg" alt="Ring-Ring For You"/>
        <p>Op de Voor U pagina worden datavisualisaties getoond die relevant zijn voor de betreffende persoon die ingelogd is. In dit voorbeeld ligt de focus op tijdstippen. Hier wordt met D3 een stackedbarchart getoond. De gekleurde bars kunnen weggefiltered worden door op de betreffende filter te klikken aan de rechterkant. Daarnaast is het mogelijk om de data te filteren op dagen in plaats van tijdstippen. Naast de stacked barchart worden er ook andere data gevisualiseerd in een simpel leesbar vak en een piechart die ook met D3 ontworpen is.</p>
        <h3>Kaart pagina</h3>
        <img src="/RingRing4.jpg" alt="Ring-Ring Map"/>
        <p>Op deze pagina kunnen de beleidsmakers de routes uitstippelen per tijdstip. Er wordt gebruik gemaakt van kleurcodes voor de nachten, spitsuren en overdag (blauw, rood en geel)</p>
        <h3>Feedback pagina</h3>
        <img src="/RingRing5.jpg" alt="Ring-Ring Feedback"/>
        <p>Op de feedback pagina krijgen de beleidsmakers een overzicht te zien van alle binnen gekregen feedback. Hier worden verschillende gegevens getoont zoals afstand, datum en de feedback zelf. Het is mogelijk om de feedback te filteren op soort dag en feedbackscore. Daarnaast is het mogelijk om de feedback door te versturen naar een mede beleidsmaker wanneer de knop 'selecteer' wordt gebruikt.</p>
        <h3>Feedback pagina - Versturen van feedback #1</h3>
        <img src="/RingRing6.jpg" alt="Ring-Ring Sent Feedback 1"/>
        <h3>Feedback pagina - Versturen van feedback #2</h3>
        <img src="/RingRing7.jpg" alt="Ring-Ring Sent Feedback 2"/>
</ProjectPage>