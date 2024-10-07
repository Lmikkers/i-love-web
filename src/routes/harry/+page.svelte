<script>
    import Harry from '$lib/harry.svelte';
    let mood = "neutraal"; // default mood
    // let harryMood = "happy"; // Define the mood you want to pass
    
    function setTwerkMood() {
        mood = "twerk";
        console.log(mood)
    }
    function setSombreroMood() {
        mood = "boos";
    }
    function setNeutralMood() {
        mood = "neutraal";
    }
</script>

<main>
    <h1>Hier komt Harry</h1>

    <div class="halloharry">
        <!-- <a class="harryknop" href="#"> -->
            <Harry {mood} />
        <!-- </a>     -->
    </div>

    <button on:click={setNeutralMood}>Hi Harry!</button>
    <button on:click={setTwerkMood}>Twerk Harry</button>
    <button on:click={setSombreroMood}>Sombero Harry</button>
    
</main>  
  
<style>
    button {
        border: none;
        font-size: 1rem;
        padding: .8rem 1rem;
        border-radius: 4px;
        cursor: pointer;
        background-color: #FA89B9;
        color: white;
        transition: ease-out .5s;
    }
    button:hover,
    button:focus {
        background-color: #eb659c;
    }
</style>