<script>
    import MarcoHeader from '/src/Components/Resources/MarcoSVG.svelte';
    import FijanHeader from '/src/Components/Resources/FijanSVG.svelte';

    let y;
    // let CTAButton;

    let enableStickyButton = false;
    let ctaButtonContent = 'Neem contact met me op!';

    window.addEventListener('scroll', function(){
        if(y < 70){
            enableStickyButton = false;
            ctaButtonContent = 'Neem contact met me op!'
        }
        else{
            enableStickyButton = true;
            ctaButtonContent = '';       
        }
    })



</script>
<style>
    img{
        position: absolute;
        right: 10%;
        bottom: 0;
        height: 70vh;
        width: 20em;
        animation: hoverInImageOnLoad 2s ease-in-out 0s 1 normal forwards ;
        z-index: 10;
    }
    h1{
        font-size: 4em;
        color: white;
        margin: 0;
        z-index: 10;
    }
    h2{
        color:white;
        font-size: 1.3em;
        margin-bottom: 0;
        font-weight: 100;
        text-transform: uppercase;
        z-index: 10;
    }
    article{
        position: absolute;
        max-width: 50em;
        margin-left: 3rem;
        padding-left: 10%;
        padding-bottom: 7rem;
        bottom: 0;
        opacity: 0;
        animation: hoverInArticleOnLoad 2s ease-in-out 1s 1 normal forwards ;
        box-sizing: border-box;
        z-index: 10;
    }
    p{
        color:white;
        z-index: 10;
    }

    a{
        display: flex;
        background: #ed4c4c;
        background: linear-gradient(120deg, #ed4c4c, #f9ac39, rgba(237,76,76,1));
        background-size: 200%;
        color: white;
        text-decoration: none;
        text-align: center;
        align-self: center;
        width: 22rem;
        height: 3em;
        line-height: 3em;
        box-shadow: 0px 0px 3px white;
        border-radius: 2em;
        display: block;
        margin: 2rem 0;
        text-align: center;
        z-index: 9999;
        position: fixed;
        bottom: 1rem;
        right: 50%;
        transform: translateX(50%);
        opacity: 0;
        animation: hoverInButtonOnLoad 1s ease-in-out 3s 1 normal forwards ;
        transition: all .5s ease-in-out;
        font-size: 1.3rem;
    }

    a:hover{
        background-position: right;
        box-shadow: 0px 0px 10px white;
    }

    a>i{
        padding-left: 1rem;
        display: inline;
    }

    .stickyCTAButton{
        position: fixed;
        bottom: 2rem;
        right: 3%;
        width: 3.5rem;
        height: 3.5rem;
        line-height: 3.5rem;
        font-size: 1.2rem;
    }

    .stickyCTAButton>i{
        padding:0;
    }

    @keyframes hoverInArticleOnLoad{
        0%{
            opacity: 0;
            bottom: -3em;
        }

        100%{
            opacity: 1;
            bottom: 0;
        }
    }

    @keyframes hoverInButtonOnLoad{
        0%{
            opacity: 0;
        }

        100%{
            opacity: 1;
        }
    }

    @keyframes hoverInImageOnLoad{
        0%{
            opacity: 0;
            margin-top: 65vh;
        }

        50%{
        }

        100%{
            opacity: 1;
            margin-top: 55vh;
        }
    }
</style>

<MarcoHeader></MarcoHeader>
<FijanHeader></FijanHeader>

<svelte:window bind:scrollY={y}/> 

<article>
    <h2>Marco Fijan</h2>
    <h1>Website en User Interface Developer</h1>
    <p>Ik design en creeër webapplicaties die gebruikers fijn vinden om te gebruiken. Door mijn kennis van CSS3, HTML5, ES6 en frameworks te combineren lever ik symantisch correcte website die daarnaast modern, responsive en snel werken</p>
    <a href="#contact" class="{enableStickyButton ? 'stickyCTAButton': ''}">{ctaButtonContent}<i class="far fa-calendar-check"></i></a>
</article>

<img src="/src/Images/IntroImage.png" alt="IntroImage"/>
