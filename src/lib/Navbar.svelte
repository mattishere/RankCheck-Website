<nav>
    <a class="name" href="">RankCheck</a>

    <ul>
        <li><a href="/discord" target="_blank"><i class="fa-brands fa-discord"></i><span>Discord</span></a></li>
        <li><a href="/invite" target="_blank" class="invite"><i class="fa-regular fa-envelope"></i>Invite</a></li>
    </ul>
</nav>

<style>
    nav {
        z-index: 12345;
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        width: 100%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 1rem;
        color: var(--text);
        background-color: var(--background);
    }

    nav ul {
        display: flex;
        list-style: none;
        gap: 1rem;
    }


    nav a {
        text-decoration: none;
        color: var(--text);
        font-size: 1.4rem;
    }

    nav a i {
        margin-right: 0.25rem;
    }

    nav .name {
        font-size: 1.7rem;
    }

    .invite {
        background-color: var(--secondary);
        padding: 0.5rem 1rem;
        border-radius: 15px;
        transition: .2s;
    }

    @media (max-width: 550px) {
        nav {
            padding: 1rem 0.5rem;
        }

        nav .name {
            font-size: 1.5rem;
        }

        nav a {
            font-size: 1.2rem;
        }

        nav a span {
            display: none;
        }

        nav a i {
            margin-right: 0;
        }
    }

    @media (max-width: 450px) {
        nav .name {
            font-size: 1.5rem;
        }

        nav a {
            font-size: 1.2rem;
        }

        .invite {
            padding: 0.5rem 0.8rem;
        }
    }

    @media (max-width: 350px) {
        nav ul {
            gap: 5px;
        }

        nav .name {
            font-size: 1.1rem;
        }

        nav a {
            font-size: 1rem;
        }

        .invite {
            padding: 0.4rem 0.7rem;
        }
    }

    @media (max-width: 235px) {
        nav {
            padding: .7rem 0.5rem;
        }

        nav ul {
            gap: 5px;
        }

        nav .name {
            font-size: .9rem;
        }

        nav a {
            font-size: .8rem;
        }

        .invite {
            padding: 0.25rem 0.5rem;
        }
    }
</style>