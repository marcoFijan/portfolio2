<script>
    import MarcoHeader from '/src/Components/Resources/MarcoSVG.svelte';
    import FijanHeader from '/src/Components/Resources/FijanSVG.svelte';
</script>
<style>
    img{
        position: absolute;
        right: 0;
        bottom: 0;
        height: 70vh;
        animation: hoverInImageOnLoad 2s ease-in-out 0s 1 normal forwards ;
    }
    h2{
        font-size: 4em;
        color: white;
        margin: 0;
    }
    h3{
        color:white;
        font-size: 1.5em;
    }
    article{
        position: absolute;
        max-width: 40em;
        margin-left: 2em;
        height: 55vh;
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
        width: 12em;
        height: 1em;
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

<MarcoHeader></MarcoHeader>
<FijanHeader></FijanHeader>

<article>
    <h3>Dark mode? Nice!</h3>
    <h2>Website en User Interface Developer</h2>
    <p>Ik design en creeër webapplicaties die gebruikers fijn vinden om te gebruiken. Door mijn kennis van CSS3, HTML5, ES6 en frameworks te combineren lever ik symantisch correcte website die daarnaast modern, responsive en snel werken</p>
    <a href="#contact">Neem contact met me op!</a>
</article>

<img src="/src/Images/IntroImage.png" alt="IntroImage"/>