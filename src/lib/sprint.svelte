<script>
    export let number;
    export let title;

    // Splits de titel op woorden
    let titleWords = title.split(' ');
</script>

<article>
    <h3>{number}</h3>
    {#each titleWords as word}
        <h2>{word}</h2>
    {/each}
</article>

<style>
    article {
        position: relative;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 100%;
        padding: 1rem;
        background: #D9D9D9;
        border-radius: 8px;
        min-height: 15.75rem;
        background-color: #2B4176;
        color: #FF7F3B;
    }
    h2, 
    h3 {
        font-family: var(--detailFont);
        text-transform: uppercase;
        letter-spacing: .2rem;
        text-align: center;
    }
    h3 {
        position: absolute;
        top: 1rem;
        left: 1rem;
        font-size: 2rem;
    }
</style>