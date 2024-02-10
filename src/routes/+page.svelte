<script>
    import Navbar from '$lib/Navbar.svelte';
</script>

<Navbar />


<section id="home" class="center">
    <div class="section-content">
        <img src="/rankcheck-transparent.png" alt="logo" />
        <div class="text">
            <h1>RankCheck</h1>
            <p>The Overwatch 2 stats bot that you need in your Discord server!</p>
            <div class="links">
                <a href="/invite" class="invite-btn" target="_blank">Invite</a>
                <a href="#discord" class="server-btn">Discord Server</a>
                <a href="https://top.gg/bot/1189356164132130956" target="_blank">Top.gg</a>
                <a href="#tos">Terms of Service</a>
                <a href="#privacy">Privacy Policy</a>
            </div>
        </div>
    </div>

    <a class="scroll-prompt" href="#preview">
        <i class="fa-solid fa-arrow-down"></i>
        Command preview
    </a>
</section>

<section id="preview" class="center">

    <div class="section-content">
        <img src="/preview.jpg" alt="">
        <div class="info">
            <h2>Check Overwatch 2 ranks in Discord!</h2>
            <p>Easily check others' PC and console stats by entering their Battle.net tag!</p>
        </div>
    </div>

    <a class="scroll-prompt" href="#discord">
        <i class="fa-solid fa-arrow-down"></i>
        Discord Server
    </a>
</section>

<section id="discord" class="center">
    <div class="section-content">
        <iframe src="https://discord.com/widget?id=1190455944975483051&theme=dark" allowtransparency="true" frameborder="0" sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"></iframe>
        <div class="info">
            <h2>Join our Discord server!</h2>
            <p>Meet new players, learn about new features early, suggest new ones and report issues you encounter!</p>
            <div class="links">
                <a href="/discord" target="_blank">Discord Server</a>
            </div>
        </div>
    </div>
    <a class="scroll-prompt" href="#team">
        <i class="fa-solid fa-arrow-down"></i>
        The Team
    </a>
</section>

<section id="team" class="center">
    <div class="section-content">
        <div class="info">
            <h2>The team behind RankCheck</h2>
            <div class="members">
                <div class="member">
                    <h3>Matt</h3>
                    <p class="role">Developer & Owner</p>
                    <ul class="accounts">
                        <li><a href="https://matthere.net" target="_blank"><i class="fa-solid fa-globe"></i>Personal website</a></li>
                        <li><a href="https://github.com/mattishere" target="_blank"><i class="fa-brands fa-github"></i>GitHub</a></li>
                        <li><p><i class="fa-brands fa-discord"></i>@matthereatm</p></li>
                    </ul>
                </div>
                <div class="member">
                    <h3>Faith</h3>
                    <p class="role">Artist</p>
                    <ul class="accounts">
                        <li><a href="https://www.instagram.com/faith.art28" target="_blank"><i class="fa-brands fa-instagram"></i>Instagram</a></li>
                        <li><p><i class="fa-brands fa-discord"></i>@faith.art28</p></li>
                    </ul>
                </div>
            </div>
            <p>Join our <a href="#discord">Discord</a> to meet the Staff and Advisors!</p>
        </div>
    </div>
    <a class="scroll-prompt" href="#tos">
        <i class="fa-solid fa-arrow-down"></i>
        Terms of Service
    </a>
</section>

<section id="tos" class="center">
    <div class="section-content">
        <div class="info">
            <h2>Terms of Service</h2>
            <ul>
                <li>By using RankCheck, you agree to the Terms of Service written on this page.</li>
                <li>Users are expected to use the bot for legitimate and legal reasons.</li>
                <li>The bot (RankCheck) may go offline for a certain period of time in case of maintenance, updates or system failure.</li>
                <li>The RankCheck team reserves the right to terminate access to the bot in case of not following our outlined rules and Terms of Service.</li>
                <li>RankCheck is not affiliated with Blizzard Entertainment or any of its partners.</li>
                <li>RankCheck only holds publicly accessible Overwatch statistics for the purposes of caching.</li>
            </ul>
        </div>
    </div>
    <a class="scroll-prompt" href="#privacy">
        <i class="fa-solid fa-arrow-down"></i>
        Privacy Policy
    </a>
</section>

<section id="privacy" class="center">
    <div class="section-content">
        <div class="info">
            <h2>Privacy Policy</h2>
            <ul>
                <li>This privacy policy is designed to outline the ways RankCheck handles the data it is given.</li>
                <li>RankCheck only holds publicly accessible Overwatch statistics for the purposes of caching (lifetime of 1 hour) and is not stored on long-term storage.</li>
            </ul>
        </div>
    </div>
</section>


<style>
    section {
        position: relative;
        overflow: hidden;
        display: flex;
        flex-direction: column;

        width: 100vw;
        height: 100vh;
    }

    .section-content {
        flex-grow: 1;
        display: flex;
        flex-direction: row;
        align-items: center;
    }

    section .scroll-prompt {
        position: absolute;
        bottom: 0;
        width: 100%;
        text-align: center;
        text-decoration: none;
        padding: 1rem;
        font-size: 1.2rem;
    }

    .center {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .info {
        display: flex;
        flex-direction: column;
    }
    .info h2 {
        font-size: 2.5rem;
    }
    .info p {
        font-size: 1.5rem;
    }

    /* Hero */

    #home img {
        width: 500px;
    }

    .text {
        display: flex;
        flex-direction: column;
    }
    .text h1 {
        font-size: 4rem;
    }

    .text p {
        font-size: 2rem;
    }

    .links {
        display: flex;
        flex-direction: row;
        gap: 20px;
        margin-top: 20px;
    }

    .links a {
        padding: 1rem;
        border-radius: 15px;
        border: 1px solid var(--text);
        text-decoration: none;
        font-size: 1.3rem;
        transition: .2s;
    }
    .links a:hover {
        background-color: var(--primary);
        transition: .2s;
    }

    /* Preview */

    #preview img {
        width: 500px;
        border-radius: 30px;
        box-shadow: 1px 1px 8px rgba(0, 0, 0, 0.4);
        margin: .5rem;
    }

    #preview .info, #discord .info {
        margin-left: 20px;
    }

    /* Discord */

    #discord iframe {
        border-radius: 30px;
        box-shadow: 1px 1px 8px rgba(0, 0, 0, 0.4);
        width: 450px;
        height: 500px;
        margin: .5rem;
    }

    /* Team */

    #team .info, #tos .info, #privacy .info {
        align-items: center;
        gap: 50px;
    }

    .members {
        display: flex;
        flex-direction: row;
        gap: 50px;
        margin: .5rem;
    }

    .member {
        width: 500px;
        height: 250px;

        border: 2px solid var(--text);
        background-color: var(--background);
        box-shadow: 1px 1px 8px rgba(0, 0, 0, 0.4);
        display: flex;
        flex-direction: column;
        text-align: center;
        padding: 2rem;
    }

    .member h3 {
        font-size: 3rem;
        text-decoration: underline;
    }

    .member .role {
        font-size: 1.8rem;
        margin-bottom: 1rem;
    }

    .member .accounts {
        display: flex;
        flex-direction: column;
        list-style: none;
    }

    .member .accounts li {
        font-size: 1.5rem;
    }

    .member .accounts li a {
        text-decoration: underline;
    }

    .member .accounts li a i, .member .accounts li p i {
        margin-right: .25rem;
    }

    /* Terms of Service & Privacy Policy */
    #tos ul, #privacy ul {
        margin: 1.25rem;
        font-size: 1.5rem;
        width: 70%;
    }
    #tos ul li, #privacy ul li {
        margin-bottom: .5rem;
    }


    /* Responsitivity */
    @media (max-width: 1330px) {
        #home img {
            width: 400px;
        }
    }
    @media (max-width: 1230px) {
        #home img {
            width: 350px;
        }
        #home .links a {
            font-size: 1.1rem;
        }
    }
    @media (max-width: 1090px) {
        #home img {
            width: 350px;
        }
        #home h1 {
            font-size: 3rem;
        }
        #home p {
            font-size: 1.75rem;
        }
        #home .links {
            gap: 10px;
        }

        #team .info {
            text-align: center;
        }

        .members {
            flex-direction: column;
            align-items: center;
            gap: 20px;
            width: 100%;
            margin: 0;
        }

        .member {
            width: 90%;
            height: 30%;
        }
    }

    @media (max-width: 1050px) {
        #home .section-content {
            flex-direction: column;
            justify-content: center;
        }

        #home img {
            width: 250px;
        }
        #home .section-content .text {
            text-align: center;
        }

        #home .section-content .links {
            justify-content: center;
        }

        .server-btn {
            display: none;
        }

        #preview img {
            width: 350px;
        }

        #preview h2 {
            font-size: 1.7rem;
        }

        #preview p {
            font-size: 1.25rem;
        }
    }

    @media (max-width: 850px) {
        #discord iframe {
            width: 400px;
            height: 450px;
        }

        #discord h2 {
            font-size: 2rem;
        }

        #discord p {
            font-size: 1.25rem;
        }

        #discord .links a {
            padding: .75rem;
            font-size: 1.1rem;
        }

        #team .members {
            gap: 10px;
        }

        #tos ul, #privacy ul {
            width: 90%;
        }
    }

    @media (max-width: 700px) {
        #home img {
            width: 200px;
        }

        #home h1 {
            font-size: 2.5rem;
        }
        #home p {
            font-size: 1.25rem;
        }

        #home .links {
            gap: 5px;
        }
        #home .links a {
            padding: .75rem;
            font-size: 1rem;
        }

        #preview .section-content {
            flex-direction: column;
            justify-content: center;
        }

        #preview .section-content .info {
            margin: 0;
            margin-top: 1rem;
            text-align: center;
        }

        #discord iframe {
            width: 300px;
            height: 400px;
        }

        #discord h2 {
            font-size: 1.75rem;
        }

        #discord p {
            font-size: 1.1rem;
        }

        #discord .links a {
            padding: .5rem;
            font-size: 1.05rem;
        }

        .member h3 {
            font-size: 2rem;
        }

        #tos ul, #privacy ul {
            font-size: 1.2rem;
            margin: 0;
        }
    }

    @media (max-width: 594px) {
        #home img {
            width: 175px;
        }
        #home h1 {
            font-size: 2rem;
        }
        #home p {
            font-size: 1.1rem;
        }

        #discord iframe {
            width: 240px;
            height: 350px;
        }

        #discord h2 {
            font-size: 1.5rem;
        }

        #discord p {
            font-size: 0.95rem;
        }

        .member h3 {
            font-size: 1.5rem;
        }

        #team p {
            font-size: 1.2rem;
        }

        #team li p, #team li a {
            font-size: 1.2rem;
        }

        #team h2 {
            font-size: 1.9rem;
        }

        #team .info {
            gap: 10px;
        }

        #tos ul, #privacy ul {
            font-size: 1rem;
            margin: .5rem;
        }

        #tos ul li, #privacy ul li {
            margin-bottom: .3rem;
        }

        #tos h2, #privacy h2 {
            font-size: 1.9rem;
        }

        
    }

    @media (max-width: 500px) {
        #discord .section-content {
            flex-direction: column;
            justify-content: center;
        }

        #discord iframe {
            width: 80%;
            margin: .2rem;
        }

        #discord .info {
            margin: 0;
            margin-top: 1rem;
            text-align: center;
        }
        
        #discord .links {
            justify-content: center;
        }

        #tos ul, #privacy ul {
            margin: 0;
        }

        #tos ul li, #privacy ul li {
            margin-bottom: .2rem;
        }
    }

    @media (max-width: 450px) {
        .invite-btn {
            display: none;
        }

        #preview img {
            width: 300px;
        }

        #preview h2 {
            font-size: 1.3rem;
        }

        #preview p {
            font-size: 1rem;
        }

        .member {
            padding: .5rem;
            width: 70%;
        }

        #team h2 {
            font-size: 1.5rem;
        }


    }

    @media (max-width: 390px) {
        #home img {
            width: 120px;
        }
        #home h1 {
            font-size: 1.75rem;
        }
        #home p {
            font-size: .9rem;
        }

        #home .links a {
            padding: .5rem;
            font-size: .9rem;
        }
    }

    @media (max-width: 330px) {
        #home img {
            width: 100px;
        }
        #home h1 {
            font-size: 1.5rem;
        }
        #home p {
            font-size: .8rem;
        }

        #home .links a {
            padding: .4rem;
            font-size: .8rem;
        }


        #preview img {
            width: 250px;
        }

        #preview h2 {
            font-size: 1.1rem;
        }

        #preview p {
            font-size: .9rem;
        }

        #discord iframe {
            width: 90%;
            height: 45%;
            border-radius: 10px;
        }
    }
</style>