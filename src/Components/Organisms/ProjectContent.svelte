<script>
    export let title;
    export let description;
    export let projectType;
    export let projectYear;
    export let githubLink;
    export let liveLink;
    export let targetAudience;
</script>

<style>
    strong{
        font-weight: bold;
    }

    h1{
        margin: 0;
        padding: 0;
        font-size: 3rem;
    }
</style>

<h1>{title}</h1>
<p><strong>Project jaar: {projectYear}</strong></p>
<p><strong>Projectdoel: {projectType}</strong></p>
<p><strong>Doelgroep: {targetAudience}</strong></p>
<h2>Over {title} project</h2>
<p>{description}</p>
<h3>Github Link</h3>
<a href={githubLink}>{githubLink}</a>
<h3>Live demo link</h3>
<a href={liveLink}>{liveLink}</a>
