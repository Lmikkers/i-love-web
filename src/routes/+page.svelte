<script>
    import Sprint from '$lib/sprint.svelte';

    let sprintNumber = '13';
    let sprintTitle = 'Your tribe for life';

    let sprints = [
    { title: '13', number: 'Your tribe for life' },
    { title: '14', number: 'Lose your head' },
    { title: '15', number: 'Choices Choices' },
    { title: '16', number: 'Don’t repeat your self' },
    { title: '17', number: 'User needs' },
    { title: '18', number: 'Release Candidate' },
    { title: '19', number: 'Free space' },
    { title: '20', number: 'Final sprint' },
  ];
</script>

<header>

</header>

<main>
    <section>
        <h2>Sprints</h2>

        <section class="sprints">
            <!-- <Sprint title={sprintTitle} number={sprintNumber} /> -->

            <!-- Itereer over de lijst van sprints en voeg dynamisch meerdere Sprint componenten toe -->
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