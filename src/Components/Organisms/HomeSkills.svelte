<script></script>
<style>
    article{
        background: #f1f1f1;;
        min-height: 100vh;
        width: 100%;
        padding: 5rem 10%;
        box-sizing: border-box;
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

    .skillImageWrapper{
        width: 60%;
        min-width: 900px;
        height: 80vh;
        margin: 0 auto;
        box-sizing: border-box;
        position: relative;
        display: flex;
        justify-content: center;
        transition: all 1s ease-in-out;
    }

    .skillImageWrapper img{
        width: 50%;
        min-width: 20rem;
        margin: 0 auto;
        display: block;
    }

    .skillImageWrapper>div{
        position: absolute;
        display: flex;
        width: 3rem;
        height: 3rem;
        display: absolute;
        background: linear-gradient(164deg, rgba(59,167,253,1) 0%, rgba(72,79,238,1) 100%);
        color: white;
        border-radius: 5rem;
        text-align: center;
        align-items: center;
        justify-content: center;
        box-shadow: 0px 0px 10px #adadad;
        transition: all 1s ease-in-out;
    }

    .skillImageWrapper>div p{
        font-size: .4rem;
        transition: all 1s ease-in-out;
    }

    .skillImageWrapper:hover>div{
        width: 6rem;
        height: 6rem;
    }

    .skillImageWrapper:hover>div p{
        font-size: .8rem;
    }

    /* HTML  */
    .skillImageWrapper:hover>div:nth-child(1), .skillImageWrapper:active>div:nth-child(1){
        left: 0;
        bottom: 35%;
        transform: translateY(35%);
        background: linear-gradient(164deg, rgb(249, 57, 207), rgb(207, 30, 104));
    }

    /* CSS  */
    .skillImageWrapper:hover>div:nth-child(2), .skillImageWrapper:active>div:nth-child(2){
        right: 0;
        bottom: 35%;
        transform: translateY(35%);
        background: linear-gradient(164deg, rgb(249, 57, 207), rgb(207, 30, 104));
    }

    /* JAVASCRIPT  */
    .skillImageWrapper:hover>div:nth-child(3), .skillImageWrapper:active>div:nth-child(3){
        left: 0;
        top: 35%;
        transform: translateY(-35%);
        background: linear-gradient(164deg, rgba(249,172,57,1), rgba(237,76,76,1));
    }

    /* MARVEL  */
    .skillImageWrapper:hover>div:nth-child(4), .skillImageWrapper:active>div:nth-child(4){
        right: 0;
        top: 35%;
        transform: translateY(-35%);
        background: linear-gradient(164deg, rgba(249,172,57,1), rgba(237,76,76,1));
    }

    /* FIGMA */
    .skillImageWrapper:hover>div:nth-child(5), .skillImageWrapper:active>div:nth-child(5){
        bottom: 12%;
        left: 80%;
        transform: translate(-80%, 12%);
        background: linear-gradient(164deg, rgba(249,172,57,1), rgba(237,76,76,1));
    }

    /* ILLUSTRATOR */
    .skillImageWrapper:hover>div:nth-child(6), .skillImageWrapper:active>div:nth-child(7){
        bottom: 12%;
        left: 20%;
        transform: translate(-20%, 12%);
        background: linear-gradient(164deg, rgba(249,172,57,1), rgba(237,76,76,1));
    }

    /* GITHUB */
    .skillImageWrapper:hover>div:nth-child(7), .skillImageWrapper:active>div:nth-child(7){
        top: 12%;
        left: 80%;
        transform: translate(-80%, -12%);
        background: linear-gradient(164deg, rgba(249,172,57,1), rgba(237,76,76,1));
    }

    /* SVELTE */
    .skillImageWrapper:hover>div:nth-child(8), .skillImageWrapper:active>div:nth-child(8){
        top: 12%;
        left: 20%;
        transform: translate(-20%, -12%);
    }

    /* ADOBE XD */
    .skillImageWrapper:hover>div:nth-child(9), .skillImageWrapper:active>div:nth-child(9){
        top: 0;
        left: 50%;
        transform: translateX(-50%);
    }

    /* PHOTOSHOP */
    .skillImageWrapper:hover>div:nth-child(10), .skillImageWrapper:active>div:nth-child(10){
        bottom: 0;
        left: 50%;
        transform: translateX(-50%);
    }

    /* %%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%% */


    /* HTML  */
    .skillImageWrapper>div:nth-child(1){
        left: 35%;
        bottom: 45%;
        transform: translateY(45%);
    }

    /* CSS  */
    .skillImageWrapper>div:nth-child(2){
        right: 35%;
        bottom: 45%;
        transform: translateY(45%);
    }

    /* JAVASCRIPT  */
    .skillImageWrapper>div:nth-child(3){
        left: 35%;
        top: 45%;
        transform: translateY(-45%);
    }

    /* MARVEL  */
    .skillImageWrapper>div:nth-child(4){
        right: 35%;
        top: 45%;
        transform: translateY(-45%);
    }

    /* FIGMA */
    .skillImageWrapper div:nth-child(5){
        bottom: 38%;
        left: 57%;
        transform: translate(-57%, 38%);
    }

    /* ILLUSTRATOR */
    .skillImageWrapper>div:nth-child(6){
        bottom: 38%;
        left: 43%;
        transform: translate(-43%, 38%);
    }

    /* GITHUB */
    .skillImageWrapper>div:nth-child(7){
        top: 38%;
        left: 57%;
        transform: translate(-57%, -38%);
    }

    /* SVELTE */
    .skillImageWrapper>div:nth-child(8){
        top: 38%;
        left: 43%;
        transform: translate(-43%, -38%);
    }

    /* ADOBE XD */
    .skillImageWrapper>div:nth-child(9){
        top: 40%;
        left: 50%;
        transform: translateX(-50%);
    }

    /* PHOTOSHOP */
    .skillImageWrapper>div:nth-child(10){
        bottom: 40%;
        left: 50%;
        transform: translateX(-50%);
    }

    .skillImageWrapper ul{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        list-style: none;
        padding: 0;
        padding-bottom: 1rem;
        opacity: 0;
        transition: all 1s ease-in-out;
    }

    .skillImageWrapper ul li{
        display: flex;
        align-items: center;
        padding: .5rem 0;
    }

    .skillImageWrapper ul li p{
        margin: 0;
    }

    .skillImageWrapper ul li div{
        width: 2rem;
        height: 2rem;
        border-radius: 1rem;
        margin-right: 2rem;
    }

    .skillImageWrapper:hover ul, .skillImageWrapper:active ul{
        opacity: 1;
    }

    .skillImageWrapper ul li:first-child div{
        background: linear-gradient(164deg, rgb(249, 57, 207), rgb(207, 30, 104));
    }

    .skillImageWrapper ul li:nth-child(2) div{
        background: linear-gradient(164deg, rgba(249,172,57,1), rgba(237,76,76,1));
    }

    .skillImageWrapper ul li:nth-child(3) div{
        background: linear-gradient(164deg, rgba(59,167,253,1) 0%, rgba(72,79,238,1) 100%);
    }

    @media only screen and (max-width: 900px) {
        .skillImageWrapper {
            min-width: 300px;
        }

        .skillImageWrapper img{
            min-width: 15rem;
        }
}
</style>

<article>
    <h2>Hoe ervaren ik ben</h2>
    <h1>Vaardigheden</h1>
    <section class="skillImageWrapper">
        <div><p>HTML</p></div>
        <div><p>CSS</p></div>
        <div><p>Javascript</p></div>
        <div><p>Marvel</p></div>
        <div><p>Figma</p></div>
        <div><p>Illustrator</p></div>
        <div><p>Github</p></div>
        <div><p>Svelte</p></div>
        <div><p>Adobe XD</p></div>
        <div><p>Photoshop</p></div>
        <img src="src/Images/laptopIcon.svg" alt="laptopIcon"/>
        <ul>
            <li><div></div><p>Expert</p></li>
            <li><div></div><p>Gevordered</p></li>
            <li><div></div><p>Beginner</p></li>
        </ul>
    </section>
</article>