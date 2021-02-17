<script>
    let y;
</script>
<style>
    svg {
        /* top: 50;
        right: 5; */
        padding: 0 1em 1em 20%;
        /* padding-left: 30%; */
        height: 30vh;
        max-width: 60%;
        overflow: visible; 
        -webkit-filter: drop-shadow( 0 0 0.75rem crimson);
        filter: drop-shadow( 0 0 4px white);
    }

    svg path{
        stroke-dasharray: 300;
        stroke-dashoffset: 300;
        fill: transparent;
        stroke: white;
        stroke-width: .5;
    }

    svg path:first-child{
        animation: stokeAnimation 2s ease-in-out 5s 1 normal forwards;
    }

    svg path:nth-child(2){
        animation: stokeAnimation 2s ease-in-out 5.3s 1 normal forwards;
    }

    svg path:nth-child(3){
        animation: stokeAnimation 2s ease-in-out 5.6s 1 normal forwards;
    }

    svg path:nth-child(4){
        animation: stokeAnimation 2s ease-in-out 5.9s 1 normal forwards;
    }

    svg path:nth-child(5){
        animation: stokeAnimation 2s ease-in-out 6.2s 1 normal forwards;
    }


    @keyframes stokeAnimation{
        80%{
            stroke-dashoffset: 0;
        }
        100%{
            stroke-dashoffset: 0;
            stroke-width: .1;
        }
    }

    @media only screen and (max-width: 900px){
        svg{
            height: 10vh;
        }
    }


</style>

<svelte:window bind:scrollY={y}/>

<svg style="transform: translate(0,{-y * (0.25 - 1)}px)" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 219.53 51.55"><title>Asset 6</title><g id="Layer_2" data-name="Layer 2"><g id="Layer_1-2" data-name="Layer 1"><path d="M17,12.82v8.64H38V34.27H17V50.4H0V0H41V12.82Z"/><path d="M46.37,0h17V50.4h-17Z"/><path d="M73.62,49.64a19.63,19.63,0,0,1-7.89-5.58l9.15-10.8a16.6,16.6,0,0,0,4,3.75,7.49,7.49,0,0,0,4,1.22,5.17,5.17,0,0,0,4.07-1.58A6.85,6.85,0,0,0,88.34,32V12.82H71.21V0h33.91V31q0,10.29-5.29,15.44T84.31,51.55A28.47,28.47,0,0,1,73.62,49.64Z"/><path d="M146.16,41.62H127l-3.39,8.78H106.34l22-50.4h16.71l22,50.4H149.54Zm-4.68-12.24-4.9-12.68-4.89,12.68Z"/><path d="M219.53,0V50.4h-14L186.41,27.5V50.4H169.85V0h14L203,22.9V0Z"/></g></g></svg>

<!-- <svg class="fijan" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 189.95 51.89"><path d="M30.8,30.27H10.55V51.19H0V0H33.33V8.54H10.55V21.76H30.8Z"/><path d="M50.66,51.19H40.11V0H50.66Z"/><path d="M81.07,0H91.62V35.44a17,17,0,0,1-2.16,8.63,14.79,14.79,0,0,1-6.1,5.78,19.07,19.07,0,0,1-8.9,2q-8.11,0-12.66-4.13T57.27,36.07H67.89c0,2.51.52,4.36,1.58,5.56s2.72,1.79,5,1.79a6,6,0,0,0,4.82-2.08,8.78,8.78,0,0,0,1.79-5.9Z"/><path d="M128.78,40.64H110.29l-3.52,10.55H95.55L114.61,0h9.77l19.16,51.19H132.33ZM113.13,32.1h12.8L119.5,12.94Z"/><path d="M190,51.19H179.4L158.87,17.51V51.19H148.32V0h10.55l20.57,33.75V0H190Z"/></svg> -->
