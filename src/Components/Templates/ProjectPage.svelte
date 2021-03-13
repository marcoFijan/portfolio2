<script>
    import Header from '/src/Components/Organisms/Header.svelte';
    import ProjectContent from '/src/Components/Organisms/ProjectContent.svelte';

    export let title;
    export let description;
    export let projectType;
    export let projectYear;
    export let githubLink;
    export let liveLink;
    export let targetAudience;
</script>

<style>
    article{
        background: #f1f1f1;
        height: 100vh;
        width: 100%;
        padding: 3rem 10% 1rem 10%;
        box-sizing: border-box;
        display: grid;
        grid-gap: 4rem;
        grid-template-columns: repeat(auto-fit, minmax(20em, 1fr));
        grid-template-columns: repeat(auto-fit, minmax(20em, 1fr), minmax(20em, 2fr));
    }

    article section:nth-child(2){
        overflow-y: scroll;
        background: white;
        padding: 2rem;
        -webkit-box-shadow: 0px 5px 10px 0px #cacaca;
        box-shadow: 0px 3px 10px 0px #cacaca;
        border-radius: .3rem;
    }

    /* Scrollbar styling */
    article section:nth-child(2)::-webkit-scrollbar {
        width: 12px;              
    }

    article section:nth-child(2)::-webkit-scrollbar-track {
        background: white;
        border-radius: .3rem; 
    }

    article section:nth-child(2)::-webkit-scrollbar-thumb {
        background: rgb(59,167,253);
        background: linear-gradient(164deg, rgba(59,167,253,1) 0%, rgba(72,79,238,1) 100%);
        border-radius: 2rem;
        margin: 1px;
    }

    div{
        margin-top: 2.5rem;
        text-align: center;
    }

    .goBackButton{
        color: black;
        border: 1px solid black;
        border-radius: 2rem;
        padding: .8rem 1.5rem;
        text-decoration: none;
        transition: all .5s ease-in-out;
        margin: 0 auto;
        box-shadow: 0px 0px 0px white;
        background: linear-gradient(164deg, transparent, transparent, #34caee, #b239b6);
        background-size: 300%;
        background-position: left;
    }

    .goBackButton:hover{
        /* background: rgba(59,167,253,1); */
        /* background: linear-gradient(164deg, transparent, transparent, #34caee, #b239b6); */
        color: white;
        border: 1px solid white;
        box-shadow: 0px 0px 3px white;
        background-position: right;
    }

    @media only screen and (max-width: 900px) {
        article section:nth-child(2){
            overflow-y: auto;
        }  

        article{
            height: auto;
        }

        article section:nth-child(2){
            padding: 0;
            background: transparent;
            box-shadow: none;
        }
    }

</style>

<Header></Header>
<article>
    <section>
        <ProjectContent
            title={title}
            projectYear={projectYear}
            projectType={projectType}
            description={description}
            githubLink={githubLink}
            liveLink={liveLink}
            targetAudience={targetAudience}>
        </ProjectContent>
        <div>
            <a class="goBackButton" href="/#projects">
                Ga terug naar hoofdpagina
            </a>
        </div>
    </section>
    <section>
        <h2>Ontwerp</h2>
        <slot></slot>
    </section>
</article>