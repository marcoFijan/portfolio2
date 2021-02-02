<script></script>
<style>
    article{
        background: transparent;
        min-height: 50vh;
        width: 100%;
        padding: 5rem 10%;
        box-sizing: border-box;
        color:white;
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
        font-family: 'Archivo Black', sans-serif;
    }

    ul{
        list-style: none;
        padding: 0;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

    ul li{
        /* background: transparent; */
        color: black;
        text-align: center;
        height: 18rem;
        width: 12rem;
        border-radius: 1em;
        margin: 1.5rem;
        background: white;
        box-shadow: 0px 0px 10px #5e5e5e;
        transition: transform 1s ease-in-out;
        /* transition: rotate 1s ease-in-out; */
    }

    ul li:hover{
        transform:translateY(-2.5rem) scale(1.1) rotate(1deg);
    }

    ul li:nth-child(2):hover, ul li:nth-child(4):hover, ul li:nth-child(6):hover, ul li:nth-child(8):hover{
        transform:translateY(-2.5rem) scale(1.1) rotate(-1deg);
    }

    ul li img{
        /* width: 6rem; */
        height: 6rem;
        margin: 0 auto;
    }

    ul li p{
        padding: 0 1rem 1rem 1rem;
        box-sizing: border-box;
        font-size: .8rem;
    }

</style>
<article>
    <h2>Hoe ik een ontwerpproces doorloop</h2>
    <h1>Proces</h1>

    <ul>
        <li>
            <h3>Onderzoek</h3>
            <img src="/src/Images/ProcessResearch.svg" alt="Onderzoek"/>
            <p>Onderzoek is cruciaal voor een goed ontwerp. Ik verdiep me in uw doelgroep om zo uw website in de juiste style vorm te geven</p>
        </li>
        <li>
            <h3>LoFi Schetsen</h3>
            <img src="/src/Images/ProcessLoFi.svg" alt="LoFi"/>
            <p>Om een goede hiërarchie te creeëren, ontwerp ik eerst een paar LoFi-schetsen waar geen styling wordt toegepast</p>
        </li>
        <li>
            <h3>Feedback #1</h3>
            <img src="/src/Images/ProcessFeedback.svg" alt="Feedback"/>
            <p>Uw input is belangrijk. Na de LoFi-schetsen maak ik met u een afspraak om de hiërarchie te bespreken</p>
        </li>
        <li>
            <h3>HiFi Schetsen</h3>
            <img src="/src/Images/ProcessHiFi.svg" alt="HiFi"/>
            <p>Uw feedback verwerk ik in een HiFi ontwerp waar er kleuren en styling worden toegepast</p>
        </li>
        <li>
            <h3>Feedback #2</h3>
            <img src="/src/Images/ProcessFeedback.svg" alt="Feedback"/>
            <p>We maken weer een afspraak om te controleren of u het eens bent met het ontwerp. Ook noteer ik uw feedback</p>
        </li>
        <li>
            <h3>Development</h3>
            <img src="/src/Images/ProcessDevelopment.svg" alt="Development"/>
            <p>Nadat we een overeenstemming hebben over het design, ga ik voor u aan de slag met het coderen van uw website</p>
        </li>
        <li>
            <h3>Testen</h3>
            <img src="/src/Images/ProcessTesting.svg" alt="Testen"/>
            <p>Uw website wordt getest op onder andere responsiveness, browsersupport en javascript bugs</p>
        </li>
        <li>
            <h3>Oplevering</h3>
            <img src="/src/Images/ProcessDeliver.svg" alt="Oplevering"/>
            <p>Ik loop met u door de website en we maken de afspraak rond</p>
        </li>
    </ul>
</article>

