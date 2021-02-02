<script>
    let y;
    let gradientHeader = false;

    window.addEventListener('scroll', function(){
        if(y < 600){
            gradientHeader = false;
        }
        else{
            gradientHeader = true;
        }
    })
</script>
<style>
    header{
        color: black;
        position: fixed;
        width: 100%;
        z-index: 99999;
        transition: all .5s ease-in-out;
        opacity: 0;
        background: #f1f1f1;
        -webkit-box-shadow: 0px 5px 10px 0px #cacaca;
        box-shadow: 0px 3px 10px 0px #cacaca;

    }

    .gradientHeaderTrue{
        opacity: 1;
    }

    header ul{
        list-style: none;
        display: flex;
        padding: 0 10%;
        margin: .3rem 0;
        flex-wrap: wrap;
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
        /* text-shadow: 1px 1px white; */
        cursor: pointer;
    }

</style>

<svelte:window bind:scrollY={y}/> 

<header class="{gradientHeader ? 'gradientHeaderTrue': ''}">
    <ul>
        <li>Headeritem</li>
        <li>Headeritem</li>
        <li>Headeritem</li>
        <li>Headeritem</li>
    </ul>
</header>