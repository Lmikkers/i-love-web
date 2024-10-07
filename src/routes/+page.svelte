<script>
    import Sprint from '$lib/sprint.svelte';

    let sprints = [
        { number: '13', title: 'Your tribe for life' },
        { number: '14', title: 'Lose your head' },
        { number: '15', title: 'Choices, choices' },
        { number: '16', title: 'Don’t repeat your self' },
        { number: '17', title: 'User needs' },
        { number: '18', title: 'Release Candidate' },
        { number: '19', title: 'Free space' },
        { number: '20', title: 'Final sprint' },
    ];
    // Array van kleuren
    let colors = [
        '#FF7F3B', 
        '#E42626', 
        '#223FA0', 
        '#FFE6BA', 
        '#5C0982',
        '#A8134A', 
        '#5CB5F9', 
        '#223FA0',   
    ];
</script>

<header>

</header>

<main>
    <section>
        <h2>Sprints</h2>

        <section class="sprints">
            <!-- {#each sprints as sprint (sprint.title)}
                <Sprint number={sprint.number} title={sprint.title} />
            {/each} -->

            <!-- Deze is met de kleuren, kijken of ik dit zo wil implenteren -->
            {#each sprints as sprint, i}
                <Sprint
                    title={sprint.title}
                    number={sprint.number}
                    style="color: {colors[i % colors.length]};" 
                />
            {/each}
        </section>

    </section>

    <section class="notes">
        <h2>Aantekeningen</h2>

        <section>
            <aside>
                
            </aside>
            <article>

            </article>
        </section>

    </section>
</main>


<style>
    .sprints {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: 1fr 1fr;
        grid-gap: 1rem;
        margin-bottom: 1.75rem;
    }
    section h2 {
        margin-bottom: 1.75rem;
    }
    /* --- RESPONSIVE --- */
    @media (max-width: 1024px) {
        .sprints{
            grid-template-columns: repeat(3, 1fr);
        }
    }
    /* tablet */
    @media (max-width: 768px) {
        .sprints{
            grid-template-columns: repeat(2, 1fr);
        }
    }
    /* iphone */
    @media (max-width: 480px) {
        .sprints{
            grid-template-columns: 1fr;
        }
    }
</style>