<script></script>
<style>
    article{
        background: transparent;
        min-height: 100vh;
        width: 100%;
        padding: 8rem 10%;
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

    ul{
        list-style: none;
        padding: 0;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

    ul li{
        background: transparent;
        color: black;
        text-align: center;
        height: 18rem;
        width: 12rem;
        border-radius: 1em;
        margin: 1.5rem;
        perspective: 1000px;
    }

    .innerCard{
        position: relative;
        width: 100%;
        height: 100%;
        transition: all .8s;
        transform-style: preserve-3d;
    }

    .ul li:hover .innerCard{
        transform: rotateY(180deg);
    }

    .frontCard, .backCard {
        position: absolute;
        width: 100%;
        height: 100%;
        -webkit-backface-visibility: hidden; /* Safari */
        backface-visibility: hidden;
        background: white;
    }

    .backCard{
        transform: rotateY(180deg);
    }

</style>
<article>
    <h2>Hoe ik een ontwerpproces doorloop</h2>
    <h1>Proces</h1>

    <ul>
        <li>
            <div class="innerCard">
                <div class="frontCard">
                    <h3>Onderzoek</h3>
                    <div></div>
                </div>
                <div class="backCard">
                    <h3>Onderzoek</h3>
                    <p>Voor een goed ontwerp is onderzoek cruciaal. Ik verdiep me in uw doelgroep om zo de juiste kleuren, fonts en stylen toe te passen</p>
                </div>
            </div>
        </li>
        <li>
            <h3>Lofi Schetsen</h3>
            <div></div>
        </li>
        <li>
            <h3>Feedback #1</h3>
            <div></div>
        </li>
        <li>
            <h3>Hifi Schetsen + Feedback verwerking</h3>
            <div></div>
        </li>
        <li>
            <h3>Feedback #2</h3>
            <div></div>
        </li>
        <li>
            <h3>Feedback verwerking</h3>
            <div></div>
        </li>
        <li>
            <h3>Development</h3>
            <div></div>
        </li>
        <li>
            <h3>Testen</h3>
            <div></div>
        </li>
        <li>
            <h3>Oplevering</h3>
            <div></div>
        </li>
    </ul>
</article>

