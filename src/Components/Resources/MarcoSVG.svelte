<script></script>
<style>
    h1{
        position: absolute;
        left: 2rem;
        top: 0;
        margin: 0;
        padding: 0;
        font-size: 13em;
        text-transform: uppercase;
        font-weight: 900;
        color: transparent;
        -webkit-text-stroke: 0px white;
    }
    h1::before{
        content: attr(data-text);
        position: absolute;
        top: 0;
        left: 0;
        width: 0%;
        height: 100%;
        -webkit-text-stroke: .5px white;
        overflow: hidden;
        animation: nameTransition1 2s ease-in-out 3s 1 normal forwards ;
    }

    h1::after{
        content: attr(data-text);
        position: absolute;
        top: 0;
        left: 0;
        width: 0%;
        height: 100%;
        color: white;
        overflow: hidden;
        /* transition: color ease-in 2s; */
        animation: nameTransition2 3s ease-in-out 6s 1 normal forwards ;
    }

    @keyframes nameTransition1{
        0%{
            width: 0%;
        }
        100%{
            width: 100%;
        }
    }

    @keyframes nameTransition2{
        0%{
            width: 100%;
            color: transparent;
        }
        20%{
            width: 100%;
            color:white;
        }
        30%{
            width: 100%;
            color: white;
        }
        100%{
            color:transparent;
            width:100%;
        }
    }


</style>

<h1 data-text="Marco">Marco</h1>