<h1>Link not found</h1>
<h2>Klik op de knop om weer terug te gaan</h2>
<img src="src/Images/LinkNotFound.png" alt="Link not found">
<a href="/">Ga terug naar hoofdpagina</a>

<style>
    h1, h2{
        width: 100%;
        text-align: center;
        color: white;
        font-size: 2.5rem;
    }

    h2{
        font-size: 1.5rem;
    }

    a{
        position: absolute;
        background: #ed4c4c;
        background: linear-gradient(120deg, #ed4c4c, #f9ac39, rgba(237,76,76,1));
        background-size: 200%;
        color: white;
        text-decoration: none;
        text-align: center;
        width: 22rem;
        height: 3em;
        bottom: 12vh;
        left: 50%;
        transform: translateX(-50%);
        line-height: 3em;
        box-shadow: 0px 0px 3px white;
        border-radius: 2em;
        z-index: 9999;
        /* transform: translateX(50%); */
        transition: all .5s ease-in-out;
        font-size: 1.1rem;
        display: block;
        z-index: 100000;
    }

    a:hover{
        background-position: right;
        box-shadow: 0px 0px 10px white;
    }

    img{
        position: absolute;
        bottom: 0;
        left: 50%;
        transform: translateX(-50%);
        height: 80vh;
        z-index: 1;
    }
</style>