<script>
    import Harry from '$lib/harry.svelte';
    let mood = "twerk"; // default mood
    // let harryMood = "happy"; // Define the mood you want to pass

</script>

<section>
    <Harry {mood} />
    <h1>404</h1>
    <h3>Oeps er is iets misgegaan, excuses voor het ongemak</h3>
    
    <a class="button" href="/">Terug naar home</a>
</section>

<style>
    section {
        width: 100vw;
        height: calc(100vh - 5rem);
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        gap: 1rem;
    }
    h1 {
        font-size: 5rem;
    }
    .button {
        text-decoration: none;
        background-color: var(--sprint13);
        color: #fff;
        padding: .8rem 1.3rem ;
        border-radius: 5rem;
    }
</style>