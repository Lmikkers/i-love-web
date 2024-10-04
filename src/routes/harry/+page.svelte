<script>
    import Harry from '$lib/harry.svelte';
    let mood = "neutral"; // default mood
    // let harryMood = "happy"; // Define the mood you want to pass
    
    function setTwerkMood() {
        mood = "twerk";
        console.log(mood)
    }
    function setSombreroMood() {
        mood = "sombrero";
    }
</script>

<main>
    <h1>Hier komt Harry</h1>

    <Harry {mood} />

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
    button:hover {
        background-color: #eb659c;
    }
</style>

<!-- 
<style>
.halloharry .cartoon{
    width: 8rem;
}
.cartoon{
    width: 16rem;
    filter: drop-shadow(2px 2px 2px rgba(0, 0, 0, 0.3));
}

.cartoon g, .cartoon path{
    transform-box: fill-box;
    transform-origin: center;
    transition: 200ms;
}
.fluit, .sip, .dorst, .blij, .neutraal-2, .gek, .sangry, .neutraal, .bril, .sombrero, .sjaal, .billen{
    opacity: 0;    
}
.sangry, .neutraal{
    transform-origin: center;
    animation: blink 10s infinite;
}
.arm_l, .arm_r ,.been_l ,.been_r {
        stroke-width: 6px;
        stroke-miterlimit: 10;
        fill: #c17052;
        stroke: black;
    }
.arm_l{
    transform: translateY(-20px) translateX(-10px) rotate(-55deg);
    transform-origin: right center;
}
.arm_r{
    transform: translateY(-20px) translateX(10px) rotate(55deg);
    transform-origin: left center;
}

.harry[data-mood="neutraal"] .neutraal-2 {
    opacity: 1;
}
.harry[data-mood="neutraal"] .neutraal {
    opacity: 1;
}
.harry[data-mood="neutraal"] .arm_r {
    animation: wave 20s infinite;
}


/* Mood: Blij */
.harry[data-mood="blij"] .blij {
    opacity: 1;
}

.harry[data-mood="blij"] .neutraal {
    opacity: 1;
}

.harry[data-mood="blij"] .arm_r {
    animation: wave 20s infinite;
}

/* Mood: Dorst */
.harry[data-mood="dorst"] .dorst {
    opacity: 1;
}

.harry[data-mood="dorst"] .neutraal {
    opacity: 1;
}

/* Mood: Verdrietig */
.harry[data-mood="verdrietig"] .sip {
    opacity: 1;
}

.harry[data-mood="verdrietig"] .sangry {
    opacity: 1;
}

.harry[data-mood="verdrietig"] .plant {
    opacity: 0;
}

.harry[data-mood="verdrietig"] .arm_l {
    --rotatearm: -65deg; 
    --translateXarm: -10px;
    --translateYarm: -20px;
    transform-origin: right center;
}

.harry[data-mood="verdrietig"] .arm_r {
    --rotatearm: 65deg;
    --translateXarm: 10px;
    --translateYarm: -20px;
    transform-origin: left center;
}

.harry[data-mood="verdrietig"] .arm_r,
.harry[data-mood="verdrietig"] .arm_l {
    animation: shoulders 5s infinite;
}

.harry[data-mood="verdrietig"] .pot {
    animation: sad 5s infinite;
    transform-origin: center;
}

/* Mood: Boos */
.harry[data-mood="boos"] .sip {
    opacity: 1;
}

.harry[data-mood="boos"] .sangry {
    opacity: 1;
}

.harry[data-mood="boos"] .oog_l {
    transform: rotate(45deg);
}

.harry[data-mood="boos"] .oog_r {
    transform: rotate(-45deg);
}

/* Mood: Gek */
.harry[data-mood="gek"] .gek {
    opacity: 1;
}

.harry[data-mood="gek"] .neutraal {
    opacity: 1;
}

/* Mood: Twerk */
.harry[data-mood="twerk"] .pot {
    animation: twerkbody 0.7s infinite;
    transform-origin: top;
}

.harry[data-mood="twerk"] .billen {
    opacity: 1;
    animation: twerkbody 0.7s infinite;
}

.harry[data-mood="twerk"] .bil_l {
    animation-delay: 0.2s;
    animation: twerk 0.7s infinite;
}

.harry[data-mood="twerk"] .bil_r {
    animation: twerk 0.7s infinite;
}

.harry[data-mood="twerk"] .plant {
    transform: rotateY(180deg);
    animation: twerkbody 0.7s infinite;
    transform-origin: bottom;
}

.harry[data-mood="twerk"] .been_l,
.harry[data-mood="twerk"] .been_r {
    transform: translateY(-10px);
}

.harry[data-mood="twerk"] .arm_l {
    animation: twerkarms 0.7s infinite;
    --rotatearm: 45deg;
}

.harry[data-mood="twerk"] .arm_r {
    animation: twerkarms 0.7s infinite;
    --rotatearm: -45deg;
}

.harry[data-mood="twerk"] .pot,
.harry[data-mood="twerk"] .billen,
.harry[data-mood="twerk"] .bil_l,
.harry[data-mood="twerk"] .bil_r,
.harry[data-mood="twerk"] .plant,
.harry[data-mood="twerk"] .arm_l,
.harry[data-mood="twerk"] .arm_r {
    animation-timing-function: ease-in;
}

/* Environment: Zonnig */
.harry[data-environment="zonnig"] .sombrero {
    opacity: 1;
}

.harry[data-environment="zonnig"] .plant {
    opacity: 0;
}

/* Environment: Koud */
.harry[data-environment="koud"] .sjaal {
    opacity: 1;
}

.harry[data-environment="koud"] .mond {
    opacity: 0;
}

/* Environment: Fel */
.harry[data-environment="fel"] .bril {
    opacity: 1;
}
``

@media (min-width: 1000px) {
    #tips:before {
        transform: rotate(0deg);
        top: 50%;
        left: -1.8rem;
    }
}

/* ANIMATIES */
@keyframes wave{
    0% {    
        transform: translateY(-20px) translateX(10px) rotate(55deg);
    }
    25% {
        transform: translateY(-20px) translateX(10px) rotate(55deg);
    }
    30% {
        transform: translateY(-20px) translateX(10px) rotate(-45deg);
    }
    31% {
        transform: translateY(-20px) translateX(10px) rotate(-25deg);
    }
    32% {
        transform: translateY(-20px) translateX(10px) rotate(-45deg);
    }
    35% {
        transform: translateY(-20px) translateX(10px) rotate(55deg);    
    }
    100% {
        transform: translateY(-20px) translateX(10px) rotate(55deg);
    }
}

@keyframes angry{
    0% {
        transform: rotate(var(--normaal));
    }
    50% {
        transform: rotate(var(--tril));
    }
    100% {
        transform: rotate(var(--normaal));
    }
}

@keyframes blink{
    0% {
        transform: scaleY(1);
    }
    2% {
        transform: scaleY(0.1);
    }
    4% {
        transform: scaleY(1);
    }
    100% {
        transform: scaleY(1);
    }
}

@keyframes sad{
    0% {
        transform: scale(1);
    }
    40%{
        transform: scale(1);
    }
    45% {
        transform: scale(1.01);
    }
    50% {
        transform: scale(1);
    }
    55% {
        transform: scale(1.01);
    }
    60% {
        transform: scale(1);
    }
    100% {
        transform: rotate(1);
    }
}

@keyframes shoulders{
    0%{
        transform:  translateX(var(--translateXarm)) translateY(var(--translateYarm)) rotate(var(--rotatearm));
    }
    40%{
        transform:  translateX(var(--translateXarm)) translateY(var(--translateYarm)) rotate(var(--rotatearm));
    }
    45%{
        transform:  translateX(var(--translateXarm)) translateY(calc(var(--translateYarm) + 5px)) rotate(var(--rotatearm));
    }
    50%{
        transform:  translateX(var(--translateXarm)) translateY(var(--translateYarm)) rotate(var(--rotatearm));
    }
    55%{
        transform:  translateX(var(--translateXarm)) translateY(calc(var(--translateYarm) + 5px)) rotate(var(--rotatearm));
    }
    60%{
        transform:  translateX(var(--translateXarm)) translateY(var(--translateYarm)) rotate(var(--rotatearm));
    }
    100%{
        transform:  translateX(var(--translateXarm)) translateY(var(--translateYarm)) rotate(var(--rotatearm));
    }
}

@keyframes hide{
    0%{
    transform: rotate(20deg) translate(0);    
    }
    100%{
    transform: rotate(20deg) translate(-2vw, 3rem);    
    }
}

@keyframes twerk{
    0%{
        transform: translateX(0) rotate(0) scaleY(1);
    }
    25%{
        transform: translateX(-35px) rotate(-15deg) scaleY(1.2);
    }
    50%{
        transform: translateX(0) rotate(0)  scaleY(1);
    }
    75%{
        transform: translateX(35px) rotate(15deg) scaleY(1.2);
    }
    100%{
        transform: translateX(0) rotate(0) scaleY(1);
    }
}

@keyframes twerkbody{
    0%{
        transform: rotate(0);
    }
    20%{
        transform: rotate(10deg);
    }
    50%{
        transform: rotate(0);
    }
    80%{
        transform: rotate(-10deg);
    }
    100%{
        transform: rotate(0);
    }
}

@keyframes twerkarms{
    0%{
        transform: translateX(0) rotate(var(--rotatearm));
    }
    20%{
        transform: translateX(-10px) rotate(var(--rotatearm));
    }
    50%{
        transform: translateX(0) rotate(var(--rotatearm));
    }
    80%{
        transform: translateX(10px) rotate(var(--rotatearm));
    }
    100%{
        transform: translateX(0) rotate(var(--rotatearm));
    }
}
</style> -->