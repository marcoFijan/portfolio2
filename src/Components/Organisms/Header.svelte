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
        padding: 0 2rem;
        flex-wrap: wrap;
        width: auto;
    }

    header ul li{
        padding: .5rem;
        font-weight: bold;
        background: transparent;
        transition: all .5s ease-in-out;
    }

    header ul li:hover{
        background: rgb(237,76,76);
        background: linear-gradient(120deg, rgba(237,76,76,1), rgba(249,172,57,1), rgba(237,76,76,1));
        background-size: 200%;
        border-radius: 1.5rem;
        color: white;
        cursor: pointer;
    }

</style>
<header>
    <ul>
        <li>Headeritem</li>
        <li>Headeritem</li>
        <li>Headeritem</li>
        <li>Headeritem</li>
    </ul>
</header>