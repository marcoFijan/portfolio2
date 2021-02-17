<script></script>
<style>
    article{
        background: #f1f1f1;
        min-height: 100vh;
        width: 100%;
        padding: 5rem 10%;
        box-sizing: border-box;
    }

    strong{
        font-weight: 900;
    }

    h1{
        font-size: 4rem;
        font-weight: 900;
        margin: 0;
        margin-bottom: 6rem;
    }

    h2{
        font-weight: 100;
        font-size: 1.2rem;
        margin: 0;
    }

    h3{
        font-size: 1.8rem;
        font-family: 'Archivo Black', sans-serif;
        text-align: center;
        opacity: .4;
        text-decoration: line-through;
    }

    h3:first-child{
        opacity: 1;
        text-decoration: none;
    }

    .aboutContent{
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        flex-wrap: wrap;
    }

    .aboutContent section{
        max-width: 45rem;
        margin: 0 auto;
    }

    .aboutContent p:first-child, .aboutContent p:nth-child(2), .aboutContent p:nth-child(3), .aboutContent p:nth-child(4){
        margin: 0;
    }

    .aboutContent img{
        max-width: 25rem;
        margin: 0 auto;
        border-radius: .2rem;
    }

    article>section>section{
        flex-grow: 1;
    }

    .history{
        padding: 30vh 0 20vh 0;
    }

    @media only screen and (max-width: 900px) {
        .aboutContent>section{
            padding-top: 2rem;
        }
    }
</style>

<article id="about">
    <h2>Meer informatie over de developer</h2>
    <h1>Over Marco</h1>
    <section class="aboutContent">
        <img src="src/Images/MarcoBureau.jpg" alt="Afbeelding van Marco Fijan"/>
        <section>
            <p><strong>Marco Daniël Fijan</strong></p>
            <p><strong>25 Jaar oud</strong></p>
            <p>Woonachtig in <strong>Tilburg</strong></p>
            <p>Studeert momenteel <strong>Communicatie en Multimedia Design</strong> op Hogeschool Amsterdam</p>
            
            <p>Hallo beste lezer, <br> Ik ben Marco. Nadat ik mijn havo-diploma had behaald lag mijn interesse al snel bij de ICT. Mijn eerste studie was daarom ook Informatica op Hogeschool Rotterdam. Helaas kwam ik er al snel achter dat de kwaliteit van het onderwijs op Hogeschool Rotterdam niet bij mijn persoonlijke standaarden pastten. Daarom vervolgde ik mijn HBO Informatica studie op Hogeschool Avans in Den Bosch. Nadat ik mijn propedeuse Informatica had behaald, besloot ik toch om een andere kant te kiezen. Het coderen vond ik erg leuk, maar niet leuk genoeg om dit dagen achter elkaar alleen maar te doen. Afwisseling en creativiteit is iets wat ik mistte op de studie. Uiteindelijk kwam ik terecht op een nieuwe studie, Communicatie en Multimedia Design (CMD). Hier vond ik mijn passie voor ontwerpen en developen van verschillende applicaties. Doordat ik ook vrij perfectionistisch ben ingesteld, had ik al gelijk een oog voor detail toen ik aan de studie begon. Dit hielp mij om in het begin al nette ontwerpen op te leveren.</p>
                
            <p>Naast mijn passie voor het ontwerpen en developen van websites, kan ik ook erg genieten van rust en natuur. Vooral van bergen en groene vlaktes kan ik erg genieten. Daarnaast spaar ik ook graag edelstenen en minarelen. Dit heeft ongetwijfeld te maken met mijn interesse van de natuur. Mijn vrije tijd besteed ik ook graag aan videogames met goede storytelling. Ik kan erg genieten van een goed verhaal in een compleet andere wereld.  </p>
        </section>
    </section>
    <section class="history">
        <h3>Minor: Applied Game Design, 2021</h3>
        <h3>Start Derdejaars CMD-student, 2020</h3>
        <h3>Tweedejaars CMD-student, 2019</h3>
        <h3>Propedeuse CMD, 2018</h3>
        <h3>Tweedejaars Informatica student, 2017</h3>
        <h3>Propedeuse Informatica, 2016</h3>
    </section>

</article>