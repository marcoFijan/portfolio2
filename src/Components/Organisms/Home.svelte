<script>
    import MarcoHeader from '/src/Components/Resources/MarcoSVG.svelte';
    import FijanHeader from '/src/Components/Resources/FijanSVG.svelte';

    let y;
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
    section{
        position: absolute;
        top: 0;
        background: transparent;
    }

    img{
        position: absolute;
        right: 5%;
        bottom: 0;
        margin-bottom: -40vh;
        height: 80vh;
        animation: hoverInImageOnLoad 2s ease-in-out 0s 1 normal forwards ;
        z-index: 5;
        transition: margin .6s ease-in-out;
    }

    img:hover{
        margin-bottom: -10vh;
    }



    h1{
        font-size: 3.6em;
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
        width: 22rem;
        height: 3em;
        line-height: 3em;
        box-shadow: 0px 0px 3px white;
        border-radius: 2em;
        display: block;
        margin: 2rem 0;
        z-index: 9999;
        position: fixed;
        bottom: 1rem;
        right: 50%;
        transform: translateX(50%);
        opacity: 0;
        animation: hoverInButtonOnLoad 1s ease-in-out 3s 1 normal forwards ;
        transition: all .5s ease-in-out;
        font-size: 1.1rem;
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
        bottom: 4rem;
        right: 2.2rem;
        width: 3.5rem;
        height: 3.5rem;
        line-height: 3.5rem;
        font-size: 1.2rem;
    }

    .stickyCTAButton>i{
        padding:0;
    }

    div div{
        position: absolute;
        background: white;
        opacity: .1;
        top: 100vh;
        transition: all 1s all;
        clip-path: polygon(50% 0%, 83% 12%, 100% 43%, 94% 78%, 68% 100%, 32% 100%, 6% 78%, 0% 43%, 17% 12%);
    }

    div>div:first-child{
        height: 4rem;
        width: 4rem;
        left: 10%;
        animation: sprakleAnimation 60s ease-in-out;
    }

    div>div:nth-child(2){
        height: 6rem;
        width: 6rem;
        left: 60%;
        animation: sprakleAnimation 80s ease-in-out 1s infinite;
    }

    div>div:nth-child(3){
        height: 3rem;
        width: 3rem;
        left: 80%;
        animation: sprakleAnimation 50s ease-in-out infinite;
    }

    div>div:nth-child(4){
        height: 8rem;
        width: 8rem;
        left: 30%;
        animation: sprakleAnimation 100s ease-in-out 3s infinite;
    }

    div>div:nth-child(5){
        height: 2.5rem;
        width: 2.5rem;
        left: 90%;
        animation: sprakleAnimation 40s ease-in-out 6s infinite;
    }

    div>div:nth-child(6){
        height: 2.5rem;
        width: 2.5rem;
        left: 20%;
        animation: sprakleAnimation 40s ease-in-out 3s infinite;
    }

    div>div:nth-child(7){
        height: 2rem;
        width: 2rem;
        left: 50%;
        animation: sprakleAnimation 20s ease-in-out 3s infinite;
    }

    div>div:nth-child(8){
        height: 2.5rem;
        width: 2.5rem;
        left: 30%;
        animation: sprakleAnimation 25s ease-in-out 1s infinite;
    }

    div>div:nth-child(9){
        height: 2.5rem;
        width: 2.5rem;
        left: 70%;
        animation: sprakleAnimation 28s ease-in-out 2s infinite;
    }

    @keyframes sprakleAnimation{
        0%{
            top: 100vh;
            transform: rotate(0deg);
            opacity: .1;
        }

        30%{
            top: 50vh;
            transform: rotate(180deg);
            opacity: 0.07;
        }

        100%{
            top: -10vh;
            transform: rotate(360deg);
            opacity: 0;
        }

        

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

    @media only screen and (max-width: 900px) {
        div{
            display: none;
        }
    }
</style>

<section id="home"></section>

<MarcoHeader></MarcoHeader>
<FijanHeader></FijanHeader>

<svelte:window bind:scrollY={y}/> 

<div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
</div>

<article>
    <h2>Marco Fijan</h2>
    <h1>Website en User Interface Designer & Developer</h1>
    <p>Ik design en creeër webapplicaties die gebruikers fijn vinden om te gebruiken. Door mijn kennis van CSS3, HTML5, ES6 en frameworks te combineren lever ik symantisch correcte website die daarnaast modern, responsive en snel werken</p>
    <a href="#contact" class="{enableStickyButton ? 'stickyCTAButton': ''}">{ctaButtonContent}<i class="far fa-calendar-check"></i></a>
</article>

<img style="transform: translate(0,{-y * 1}px)" src="/src/Images/IntroImage.png" alt="IntroImage"/>
