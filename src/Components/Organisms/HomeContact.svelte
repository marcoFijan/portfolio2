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

    form{
        display: flex;
        flex-direction: column;
        max-width: 50rem;
        margin: 0 auto;
    }

    form>section{
        display: flex;
        width: 100%;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-between;
    }

    form>section>section{
        display: flex;
        flex-direction: column;
        width: 47%;
    }

    form input, form textarea{
        padding: .5rem;
        border-radius: .3rem;
        border: none;
        font-size: .9rem;
        transition: all .3s ease-in-out;
        line-height: 1.5rem;
    }

    form input:focus, form textarea:focus{
        box-shadow: inset 0px 0px 5px white;
        color: black !important;
        font-size: 1.1rem;
        background: white !important;
        outline: none;
        line-height: 1.5rem;
    }

    form input:required:invalid, form textarea:required:invalid{
        color: rgba(237,76,76,.9);
    }

    form input:required:valid, form textarea:required:valid{
        color: rgb(236, 236, 236);
        background: transparent;
    }

    form label{
        padding: 1rem 0 .3rem 0;
        font-weight: 900;
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

    /* form>section>label, form>section>input{
        width: 40%;
    } */

</style>
<article id="contact">
    <h2>Neem contact met me op</h2>
    <h1>Contact</h1>
    <form>
        <section>
            <section>
                <label for="name"> Voornaam </label>
                <input type="text" id="name" name="name" required/>
            </section>
            <section>
                <label for="surname"> Achternaam </label>
                <input type="text" id="surname" name="surname" required/>
            </section>
        </section>
        <label for="email"> E-mailadres </label>
        <input type="email" id="email" name="email" required/>
        <label for="subject"> Onderwerp </label>
        <input type="text" id="subject" name="subject" required/>
        <label for="message">Uw bericht of vraag</label>
        <textarea id="message" name="message" required></textarea>
    </form>
    
    <a class="CTAButton" href="#s" >Verstuur bericht</a>

</article>

