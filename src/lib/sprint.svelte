<script>
    export let number;
    export let title;
    // For the colors
    export let style;

    // Split title words
    let titleWords = title.split(' ');
</script>

<article style={style}>
    <h4>{number}</h4>
    {#each titleWords as word}
        <h3>{word}</h3>
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
        transition: ease-out .25s;
        cursor: pointer;
    }
    article:hover {
        transform: scale(1.05);
    }
    article:nth-child(3n+2) {
        background-color: #FFE6BA;
        color: #E42626;
    }
    article:nth-child(3n+3) {
        background-color: #F44336;
        color: #FFE6BA;
    }
    article:nth-child(3n+4) {
        background-color: lightblue;
        color: #223FA0;
    }
    h3, 
    h4 {
        font-family: var(--detailFont);
        text-transform: uppercase;
        letter-spacing: .2rem;
        text-align: center;
    }
    h3 {
        font-size: 1.75rem;
    }
    h4 {
        position: absolute;
        top: 1rem;
        left: 1rem;
        font-size: 2.25rem;
    }
</style>