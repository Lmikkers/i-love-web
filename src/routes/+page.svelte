<script>
    import Sprint from '$lib/sprint.svelte';

    let sprintNumber = '13';
    let sprintTitle = 'Your tribe for life';

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
</script>

<header>

</header>

<main>
    <section>
        <h2>Sprints</h2>

        <section class="sprints">
            {#each sprints as sprint (sprint.title)}
                <Sprint number={sprint.number} title={sprint.title} />
            {/each}
        </section>

    </section>

    <section>
        <h2>Aantekeningen</h2>
    </section>
</main>

<style>
    .sprints {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-template-rows: 1fr 1fr;
        grid-gap: 1rem;
    }
</style>