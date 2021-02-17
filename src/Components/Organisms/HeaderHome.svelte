<script>
    let y;
    let gradientHeader = false;
    let hamburgerMenu = false;

    window.addEventListener('scroll', function(){
        hamburgerMenu = false;

        if(y < 600){
            gradientHeader = false;
        }
        else{
            gradientHeader = true;
        }
    });

    function checkMenuVisible(){
        console.log('check');
        console.log(hamburgerMenu);
        if (hamburgerMenu){
            
        }
    }
</script>
<style>
    header{
        color: white;
        position: fixed;
        width: 100%;
        z-index: 99999;
        transition: all .5s ease-in-out;
        opacity: 0;
        background: linear-gradient(164deg, #34caee, #4ba3e0);
        border-bottom: 1px solid white;
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
        justify-content: space-between;
    }

    header ul li{
        padding: .05rem 0 .15rem 0;
    }

    header ul li a{
        padding: .5rem 0;
        border-bottom: 1px solid transparent;
        padding-bottom: 1rem;
        transition: all .5s ease-in-out;
        color: white;
        text-decoration: none;
        font-weight: bold;
    }

    header ul li:hover a{
        border-bottom: 1px solid white;
        padding-bottom: .2rem;
    }

    .menuButton{
        position: fixed;
        display: none;
        justify-content: center;
        align-items: center;
        position: fixed;
        bottom: 2rem;
        right: 2.2rem;
        width: 3.5rem;
        height: 3.5rem;
        cursor: pointer;
        background: #4ba3e0;
        background-size: 200%;
        border-radius: 2rem;
        z-index: 9999;
        box-shadow: 0px 0px 3px white;
        transform: translateX(50%);
        transition: all .5s ease-in-out;
    }

    .menuButton:hover{
        background-position: right;
    }

    .menuButtonBurger, .menuButtonBurger::before, .menuButtonBurger::after{
        width: 1.5rem;
        height: .25rem;
        background: white;
        border-radius: 4px;
        transition: all .5s ease-in-out;
    }

    .menuButtonBurger::before, .menuButtonBurger::after{
        content: "";
        position: absolute;
    }

    .menuButtonBurger::before{
        transform: translateY(-.6rem);
    }

    .menuButtonBurger::after{
        transform: translateY(.6rem);
    }

    #hamburgerMenu{
        display: none;
    }

    .menuButton.open{
        background-position: right;
        box-shadow: 0px 0px 3px transparent;
        background: transparent;
    }

    .menuButton.open .menuButtonBurger{
        transform: translateX(-30px);
        background: transparent;
    }

    .menuButton.open .menuButtonBurger::before{
        transform: rotate(45deg) translate(21.5px, -21.5px);
        background: white;
    }

    .menuButton.open .menuButtonBurger::after{
        transform: rotate(-45deg) translate(21.5px, 21.5px);
        background: white;
    }



    @media only screen and (max-width: 900px){
        header{
            bottom: -100vh;
            padding-bottom: 5rem;
            border-top: .1rem solid white;
            box-sizing: border-box;
        }

        .menuButton{
            display: flex;
        }
        
        ul{
            flex-direction: column;
            align-items: center;
        }

        ul li{
            margin: .5rem 0;
        }
        ul li a{
            font-size: 1.2rem;
        }

        header ul li a{
            width: 100% !important;
        }

        #showNavigation{
            bottom: 0;
        }
    }
</style>

<svelte:window bind:scrollY={y}/> 

<header class="{gradientHeader ? 'gradientHeaderTrue': ''}" id="{hamburgerMenu ? 'showNavigation': ''}">
    <input type="checkbox" id="hamburgerMenu" name="hamburgerMenu" bind:checked={hamburgerMenu} >
    <label for="hamburgerMenu" class="{hamburgerMenu ? 'menuButton open': 'menuButton'}">
        <div class="menuButtonBurger"></div>
    </label>
    <ul>
        <li>
            <a href="#home">
                Home  
            </a>
        </li>
        <li>
            <a href="#projects">
                Projecten
            </a>
        </li>
        <li>
            <a href="#proces">
                Proces
            </a>
        </li>
        <li>
            <a href="#skills">
                Vaardigheden
            </a>
        </li>
        <li>
            <a href="#about">
                Over Marco
            </a>
        </li>
        <li>
            <a href="#contact">
                Contact
            </a>
        </li>
    </ul>
</header>