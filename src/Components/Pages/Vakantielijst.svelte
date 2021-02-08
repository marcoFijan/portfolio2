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
    title={'Mijn Lijstie - Vakantielijstjes'}
    projectYear={'2019'}
    projectType={'Online prototype + Responsive'}
    targetAudience={'Studenten (18-28 jaar)'}
    description={'Tijdens het vak "Project Web" moesten we een prototype ontwerpen die te gebruiken is op vakantie. Ik koos ervoor om een vakantielijstje app te maken. Deze ontwierp ik online met HTML en CSS om wat meer een uitdaging voor mezelf te maken. In deze app kunnen er als het ware verschillende vakantielijstjes gemaakt worden met wat je allemaal wilt doen. '}
    githubLink={'https://github.com/marcoFijan/projectWebV2'}
    liveLink={'https://marcofijan.github.io/projectWebV2/'}>
        <h3>Empty State</h3>
        <img src="/src/Images/LijstieEmpty.png" alt="Mijn Lijstie - Empty State"/>
        <p>Wanneer er nog niet is ingelogd en/of als er nog geen lijstjes zijn aangemaakt, wordt de empty state weergegeven</p>
        <h3>Inlogpagina</h3>
        <img src="/src/Images/LijstieSignin.png" alt="Mijn Lijstie - Inlogpagina"/>
        <p>Iedereen kan een apart account aanmaken om een je eigen vakantielijst te maken. Daarom moet er ook eerst even ingelogd worden.</p>
        <h3>Hoofdpagina</h3>
        <img src="/src/Images/LijstieHome.png" alt="Mijn Lijstie - Hoofdpagina"/>
        <p>Na het inloggen komt de gebruiker op de hoofdpagina. Hier kan de gebruiker een bestaand lijstje aanpassen, verwijderen of activeren. Ook kunnnen er nieuwe lijstjes aangemaakt worden.</p>
        <h3>Interactie bestaand lijstje</h3>
        <img src="/src/Images/LijstiePopup.jpg" alt="Mijn Lijstie - Pop-up"/>
        <p>Wanneer er op een bestaande lijst wordt geklikt, verschijnt er een popup met verschillende acties voor die lijst</p>
        <h3>Lijstie aanpassen: Rhodos</h3>
        <img src="/src/Images/LijstieEdit.png" alt="Mijn Lijstie - Lijstie aanpassen"/>
        <p>Hier kan een lijstje aangepast worden door activiteiten toe te voegen of te verwijderen</p>
        <h3>Lijstie maken</h3>
        <img src="/src/Images/LijstieNewCountry.png" alt="Mijn Lijstie - Nieuw land kiezen"/>
        <p>Wanneer er wordt gekozen om een nieuwe lijst te maken, wordt er een pagina weergegeven waar er een nieuw land gekozen worden uit de populaire landen lijst, of kan er met de hand naar een ander land gezocht worden.</p>
        <h3>Activiteiten toevoegen</h3>
        <img src="/src/Images/LijstieAdd.png" alt="Mijn Lijstie - Nieuw activiteit"/>
        <p>Nadat er een land is geselecteerd, kunnen er activiteiten worden toegevoegd. In het tekstveld worden automatisch bij het typen al aanbevelingen gedaan</p>
        <h3>Lijstie aanpassen</h3>
        <img src="/src/Images/LijstieEdit.png" alt="Mijn Lijstie - Pas activiteiten aan"/>
        <p>Activiteiten kunnen ook weer verwijderd worden of toegevoegd worden wanneer een lijstje wordt aangepast</p>
        <h3>Vakantiemodus</h3>
        <img src="/src/Images/LijstieActive.png" alt="Mijn Lijstie - Vakantiemodus"/>
        <p>Wanneer vanaf het hoofdscherm er wordt gekozen om een lijstje te activeren, wordt dit scherm weergegeven. Per activiteit is een informatieknop, kaart en route op te vragen. Ook kan de activiteit weer weggedrukt worden wanneer je deze hebt gedaan.</p>
        <h3>Infomatiepagina</h3>
        <img src="/src/Images/LijstieInfo.png" alt="Mijn Lijstie - Activiteitinformatie"/>
        <p>Per activiteiten is er een klein artikel beschikbaar met informatie over die plek.</p>
        <h3>Activiteitenkaart</h3>
        <img src="/src/Images/LijstieMap.png" alt="Mijn Lijstie - ActiviteitKaart"/>
        <p>Mits beschikbaar, wordt er een kaart getoond van deze plek of activiteit</p>
        <h3>Routekaart</h3>
        <img src="/src/Images/LijstieRoute.png" alt="Mijn Lijstie - Routekaart"/>
        <p>Het is ook mogelijk om met de Google Maps Api een route uit te stippelen om naar de activiteit te reizen</p>
</ProjectPage>