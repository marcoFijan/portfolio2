<script>
    import Header from '/src/Components/Organisms/Header.svelte';

    import MarcoHeader from '/src/Components/Resources/MarcoSVG.svelte';
    import FijanHeader from '/src/Components/Resources/FijanSVG.svelte';
    import HomeProjects from '/src/Components/Organisms/HomeProjects.svelte';
</script>
<style>
    img{
        position: absolute;
        right: 10%;
        bottom: 0;
        height: 70vh;
        width: 20em;
        animation: hoverInImageOnLoad 2s ease-in-out 0s 1 normal forwards ;
    }
    h1{
        font-size: 4em;
        color: white;
        margin: 0;
    }
    h2{
        color:white;
        font-size: 1.5em;
    }
    article{
        position: absolute;
        max-width: 40em;
        margin-left: 7%;
        padding: 2rem;
        /* height: 55vh; */
        bottom: 0;
        opacity: 0;
        animation: hoverInArticleOnLoad 2s ease-in-out 1s 1 normal forwards ;
        box-sizing: border-box;
        text-shadow: 1px 1px 2px #2c2c2c;
    }
    p{
        color:white
    }

    a{
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
        margin: 2rem 0;
        text-align: center;
    }

    a:hover{
        background-position: right;
        box-shadow: 0px 0px 10px white;
    }

    @keyframes hoverInArticleOnLoad{
        0%{
            opacity: 0;
            bottom: -3em;
            /* padding-top: 1em; */
        }

        50%{
            /* padding-top: 0; */
        }

        100%{
            opacity: 1;
            bottom: 0;
            /* padding-top: 0; */
        }
    }

    @keyframes hoverInImageOnLoad{
        0%{
            opacity: 0;
            margin-top: 65vh;
            /* padding-top: 1em; */
        }

        50%{
            /* padding-top: 0; */
        }

        100%{
            opacity: 1;
            margin-top: 55vh;
            /* padding-top: 0; */
        }
    }
</style>

<Header></Header>

<MarcoHeader></MarcoHeader>
<FijanHeader></FijanHeader>

<article>
    <h2>Dark mode? Nice!</h2>
    <h1>Website en User Interface Developer</h1>
    <p>Ik design en creeër webapplicaties die gebruikers fijn vinden om te gebruiken. Door mijn kennis van CSS3, HTML5, ES6 en frameworks te combineren lever ik symantisch correcte website die daarnaast modern, responsive en snel werken</p>
    <a href="#contact">Neem contact met me op!</a>
</article>

<img src="/src/Images/IntroImage.png" alt="IntroImage"/>

<HomeProjects></HomeProjects>