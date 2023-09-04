<script>
    import Button from "../elements/Button.svelte";
</script>

<style>
    #about-me {
        padding: 72px;
    }

    #about-me > div {
        display: grid;
        grid-template-columns: 40% 60%;
        gap: 48px;
        align-items: center;
    }

    .about-image {
        border-radius: 45px;
        height: auto;
        object-fit: cover;
        max-width: 100%;
    }

    #about-me > div > div {
        max-width: calc(100% - 48px);
        display: flex;
        flex-direction: column;
        gap: 16px;
    }

    .position {
        color: var(--pantone-orange);
    }

    .about-header {
        display: flex;
        gap: 24px;
        align-items: center;
    }

    .about-p {
        color: #000;
    }

    .about-socials {
        margin-top: 8px;
        display: flex;
        gap: 24px;
    }
    .social-icons {
        display: flex;
        gap: 16px;
        align-items: center;
    }
</style>

<div id="about-me">
    <div>
        <img src="/images/AboutPic.jpg" alt="David Genesis Pedeglorio" class="about-image"/>
        <div>
            <section class="about-header">
                <img src="/D.png" alt="Logo of David Genesis Pedeglorio" height="107px" />
                <h1 class="display">David Genesis Pedeglorio</h1>
            </section>
            <h2 class="position">Full-Stack Developer</h2>
            <p class="body-1 about-p">I am a web developer based in Bay, Laguna, Philippines. With one year of experience, I created multiple projects ranging from personal to e-commerce. I mainly speak Figma, HTML, CSS, and ReactJS for my frontend designs. For full-stack, I utilize MERN stack.</p>
            <section class="about-socials">
                <Button size="large">Let&#39;s work together</Button>
                <div class="social-icons">
                    <img src="/icons/fb.svg" alt="Facebook" height="52.92px" />
                    <img src="/icons/ig.svg" alt="Instagram" height="52.92px" />
                    <img src="/icons/linkedin.svg" alt="LinkedIn" height="52.92px" />
                    <img src="/icons/github.svg" alt="GitHub" height="52.92px" />
                </div>
            </section>
        </div>
    </div>
    
</div>
