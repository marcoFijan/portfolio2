<script>
    // Binded variables 
    let form;
    let status;
    
    window.addEventListener("DOMContentLoaded", function() {

    // get the form elements defined in your form HTML above

    // var button = document.getElementById("my-form-button");
    // var status = document.getElementById("my-form-status");

    // Success and Error functions for after the form is submitted

        function success() {
            form.reset();
            status.innerHTML = "Uw bericht is succesvol verzonden. Ik neem zo snel mogelijk contact met u op!";
        }

        function error() {
            status.innerHTML = "Er ging iets fout, controleer uw gegevens";
        }

    // handle the form submission event

        form.addEventListener("submit", function(ev) {
            ev.preventDefault();
            let data = new FormData(form);
            ajax(form.method, form.action, data, success, error);
        });
    });

    // helper function for sending an AJAX request

    function ajax(method, url, data, success, error) {
        var xhr = new XMLHttpRequest();
        xhr.open(method, url);
        xhr.setRequestHeader("Accept", "application/json");
        xhr.onreadystatechange = function() {
            if (xhr.readyState !== XMLHttpRequest.DONE) return;
            if (xhr.status === 200) {
                success(xhr.response, xhr.responseType);
            } 
            else {
                error(xhr.status, xhr.response, xhr.responseType);
            }
        };
        xhr.send(data);
    }
</script>
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
        margin-bottom: 4rem;
    }

    h2{
        font-weight: 100;
        font-size: 1.2rem;
        margin: 0;
    }

    p{
        font-weight: bold;
        text-align: center;
        font-size: 1.1rem;
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
        font-style: italic;
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
        border: none;
        transition: all .5s ease-in-out;
        display: block;
        width: 12rem;
        /* height: 1em; */
        margin: 2rem auto;
        text-align: center;
    }

    .CTAButton:hover{
        background-position: right;
        box-shadow: 0px 0px 10px white;
    }

</style>
<article id="contact">
    <h2>Neem contact met me op</h2>
    <h1>Contact</h1>
    <p bind:this="{status}">Vul alstublieft uw gegevens in</p>
    <form action="https://formspree.io/f/mwkwzwbq" method="POST" bind:this="{form}">
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
        <button class="CTAButton" type="submit">Verstuur bericht</button>
    </form>
    
    <!-- <a class="CTAButton" href="#s" >Verstuur bericht</a> -->

</article>

