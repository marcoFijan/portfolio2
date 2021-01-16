<script>
</script>
<style>
    svg {
        top: 5;
        right: 5;
        width: 80%;
        overflow: visible; 
    }

    svg path{
        stroke-dasharray: 300;
        stroke-dashoffset: 300;
        fill: transparent;
        stroke: white;
        stroke-width: .1;
    }

    svg path:first-child{
        animation: stokeAnimation 1.5s ease-in-out 4s 1 normal forwards;
    }

    svg path:nth-child(2){
        animation: stokeAnimation 1.5s ease-in-out 4.3s 1 normal forwards;
    }

    svg path:nth-child(3){
        animation: stokeAnimation 1.5s ease-in-out 4.6s 1 normal forwards;
    }

    svg path:nth-child(4){
        animation: stokeAnimation 1.5s ease-in-out 4.9s 1 normal forwards;
    }

    svg path:nth-child(5){
        animation: stokeAnimation 1.5s ease-in-out 5.2s 1 normal forwards;
    }


    @keyframes stokeAnimation{
        to{
            stroke-dashoffset: 0;
        }
    }


</style>

<svg class="fijan" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 189.95 51.89"><path d="M30.8,30.27H10.55V51.19H0V0H33.33V8.54H10.55V21.76H30.8Z"/><path d="M50.66,51.19H40.11V0H50.66Z"/><path d="M81.07,0H91.62V35.44a17,17,0,0,1-2.16,8.63,14.79,14.79,0,0,1-6.1,5.78,19.07,19.07,0,0,1-8.9,2q-8.11,0-12.66-4.13T57.27,36.07H67.89c0,2.51.52,4.36,1.58,5.56s2.72,1.79,5,1.79a6,6,0,0,0,4.82-2.08,8.78,8.78,0,0,0,1.79-5.9Z"/><path d="M128.78,40.64H110.29l-3.52,10.55H95.55L114.61,0h9.77l19.16,51.19H132.33ZM113.13,32.1h12.8L119.5,12.94Z"/><path d="M190,51.19H179.4L158.87,17.51V51.19H148.32V0h10.55l20.57,33.75V0H190Z"/></svg>
