<style>
    header{
        color: black;
        position: fixed;
        width: 100%;
        z-index: 99999;
        transition: all .5s ease-in-out;
        background: linear-gradient(180deg, rgb(255, 255, 255), rgba(255, 255, 255, 0));
    }

    header ul{
        list-style: none;
        display: flex;
        padding: 0 10%;
        flex-wrap: wrap;
        width: auto;
        margin: .3rem;
    }

    header ul li {
        padding: .5rem 0;
    }

    header ul li a{
        font-weight: bold;
        border-bottom: 1px solid transparent;
        padding-bottom: 1rem;
        transition: all .5s ease-in-out;
        text-decoration: none;
        color: black;
    }

    header ul li:hover a{
        border-bottom: 1px solid black;
        padding-bottom: .3rem;
        cursor: pointer;
    }

    @media only screen and (max-width: 900px) {
      header ul{
        padding-right: 1rem !important;
        padding-left: 1rem !important;
      }
  }

</style>
<header>
    <ul>
        <li>
            <a href="/">
                Ga terug naar hoofdpagina
            </a>
        </li>
    </ul>
</header>