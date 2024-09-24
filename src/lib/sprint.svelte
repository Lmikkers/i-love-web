<script>
    export let number;
    export let title;
</script>

<article>
    <h3>{number}</h3>
    <h2>{title}</h2>
</article>

<style>
    article {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 100%;
        padding: 1rem;
        background: #D9D9D9;
        border-radius: 8px;
        min-height: 14rem;
    }
    article h2 {
        font-family: var(--detailFont);
        text-transform: uppercase;
        letter-spacing: .2rem;
        text-align: center;
    }
</style>