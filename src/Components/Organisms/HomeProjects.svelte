<script></script>
<style>
    article{
        background: #f1f1f1;;
        margin-top: 40vh;
        min-height: 100vh;
        width: 100%;
        padding: 8rem 10%;
        box-sizing: border-box;
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
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(25em, 1fr));
        grid-gap: 3rem;
    }

    ul li {
        /* height: 30em; */
        color: white;
        -webkit-box-shadow: 0px 5px 10px 0px #cacaca;
        box-shadow: 0px 3px 10px 0px #cacaca;
        border-radius: .3rem;
        transition: all .5s ease-in-out;
    }

    ul li:first-child{
        background-image: url("src/Images/projectPlaceholder.svg");
        background-position: center;
        background-size: cover;
        border-radius: .3rem;
        height: 20rem;
    }

    ul li{
        background-image: url("src/Images/projectPlaceholder.svg");
        background-position: center;
        background-size: cover;
        border-radius: .3rem;
        height: 20rem;
        transform: scale(1);
    }

    ul li:hover{
        transform: scale(1.05);
    }

    ul li div{
        position: absolute;
        padding: 2rem 4rem;
        box-sizing: border-box;
        /* background: linear-gradient(120deg, rgba(237,76,76,1), rgba(249,172,57,1)); */
        background: linear-gradient(164deg, rgba(59,167,253,1) 0%, rgba(72,79,238,1) 100%);
        height: 100%;
        width: 100%;
        opacity: 0;
        transition: all .5s ease-in-out;
        border-radius: .3rem;
    }

    ul li:hover div{
        opacity: .9;
    }

    ul li a{
        color: white;
    }

    ul li h3{
        position: absolute;
        font-weight: 100;
        font-size: .9em;
        margin: 0 0 .3rem 0;
        opacity: 0;
        padding: 1rem;
        box-sizing: border-box;
    }

    ul li h4{
        position: absolute;
        font-weight: bold;
        font-size: 1.5em;
        margin: 1rem 0 1rem 0;
        padding: 1rem;
        box-sizing: border-box;
        font-family: 'Archivo Black', sans-serif;
        opacity: 0;
    }

    ul li p{
        position: absolute;
        padding: 1rem;
        opacity: 0;
        bottom: 0;
    }

    ul li:hover div + h3, ul li:hover div ~ h4, ul li:hover div ~ p{
        opacity: 1;
    }

    ul li:hover div ~ h4{
        opacity: 1;
    }

    .CTAButton{
        display: block;
        background: rgb(237,76,76);
        background: linear-gradient(120deg, rgba(237,76,76,1), rgba(249,172,57,1), rgba(237,76,76,1));
        background-size: 200%;
        color: white;
        text-decoration: none;
        padding: 1em;
        box-shadow: 0px 0px 3px white;
        border-radius: 2em;
        transition: all .5s ease-in-out;
        display: block;
        max-width: 15rem;
        /* height: 1em; */
        margin: 2rem auto;
        text-align: center;
    }

    .CTAButton:hover{
        background-position: right;
        box-shadow: 0px 0px 10px white;
    }
</style>

<article>
    <h2>Mijn top ontworpen projecten</h2>
    <h1>Projects</h1>
    
    <ul>
        <li>
            <a href="something">
                <div></div>
                <h3>2019</h3>
                <h4>Dashboard Ring Ring - Datavisualisatie voor de beleidsmakers</h4>
                <p>Bekijk project </p>
            </a>
        </li>
        <li>
            <a href="something">
                <div></div>
                <h3>2019</h3>
                <h4>Dashboard Ring Ring - Datavisualisatie voor de beleidsmakers</h4>
                <p>Bekijk project </p>
            </a>
        </li>
        <li>
            <a href="something">
                <div></div>
                <h3>2019</h3>
                <h4>Dashboard Ring Ring - Datavisualisatie voor de beleidsmakers</h4>
                <p>Bekijk project </p>
            </a>
        </li>
        <li>
            <a href="something">
                <div></div>
                <h3>2019</h3>
                <h4>Dashboard Ring Ring - Datavisualisatie voor de beleidsmakers</h4>
                <p>Bekijk project </p>
            </a>
        </li>
        <li>
            <a href="something">
                <div></div>
                <h3>2019</h3>
                <h4>Dashboard Ring Ring - Datavisualisatie voor de beleidsmakers</h4>
                <p>Bekijk project </p>
            </a>
        </li>
        <li>
            <a href="something">
                <div></div>
                <h3>2019</h3>
                <h4>Dashboard Ring Ring - Datavisualisatie voor de beleidsmakers</h4>
                <p>Bekijk project </p>
            </a>
        </li>
    </ul>

    <a class="CTAButton" href="https://github.com/marcoFijan">Bekijk mijn github</a>
</article>