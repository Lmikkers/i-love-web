<nav>
    <ul>
        <li><a href="/">I-love-web</a></li>
        <li><a href="/sprints">Sprints</a></li>
        <li><a href="/contact">Contact</a></li>
    </ul>
</nav>

<slot></slot>

<style>
    nav {
        /* position: fixed; */
        background-color: #e2e2e2;
        width: 100vw;
        height: 4.5rem;
        z-index: 2;
        padding: 0rem 2rem;
        box-shadow: rgba(0, 0, 0, 0.04) 0px 3px 5px;
    }
    nav ul {
        display: flex;
        flex-direction: row;
        justify-content: center;
        align-items: center;
        gap: 1.5rem;
        width: 100%;
        height: 100%;
        list-style: none;
    }
    nav a {
        text-decoration: none;
        color: var(--fontColor);
        padding: 1.25rem;
        text-align: center;
    }
</style>