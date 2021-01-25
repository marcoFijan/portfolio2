<script></script>
<style>
    article{
        background: transparent;
        min-height: 100vh;
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

    ul li div{
        background: blue;
        width: 6rem;
        height: 5rem;
        margin: 0 auto;
    }

    ul li p{
        padding: 1rem;
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
            <div></div>
            <p>Onderzoek is cruciaal voor een goed ontwerp. Ik verdiep me in uw doelgroep om zo uw website in de juiste style vorm te geven</p>
        </li>
        <li>
            <h3>LoFi Schetsen</h3>
            <div></div>
            <p>Om een goede hiërarchie te creeëren, ontwerp ik eerst een paar LoFi-schetsen waar geen styling wordt toegepast</p>
        </li>
        <li>
            <h3>Feedback #1</h3>
            <div></div>
            <p>Uw input is belangrijk. Na de LoFi-schetsen maak ik met u een afspraak om de hiërarchie te bespreken</p>
        </li>
        <li>
            <h3>HiFi Schetsen</h3>
            <div></div>
            <p>Uw feedback verwerk ik in een HiFi ontwerp waar er kleuren en styling worden toegepast</p>
        </li>
        <li>
            <h3>Feedback #2</h3>
            <div></div>
            <p>Afspraak om te controleren of u het eens bent met het ontwerp. Daarnaast noteer ik uw feedback</p>
        </li>
        <li>
            <h3>Development</h3>
            <div></div>
            <p>Nadat we een overeenstemming hebben over het design, ga ik voor u aan de slag met de development</p>
        </li>
        <li>
            <h3>Testen</h3>
            <div></div>
            <p>Uw website wordt getest op onder andere responsiveness, browsersupport en javascript bugs</p>
        </li>
        <li>
            <h3>Oplevering</h3>
            <div></div>
            <p>Ik loop met u door de website en we maken de afspraak rond</p>
        </li>
    </ul>
</article>

