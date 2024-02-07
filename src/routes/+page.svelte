<script>

    import "../app.css"
    import globe from "../assets/globe.svg"
    import Title from "$lib/Title.svelte"
    import img from "../assets/title.jpg"
    import exp from "../assets/exp.jpg"
    import proj from '../assets/projects.jpg'
    import cover from '../assets/cover.jpg'
    import Home from "../lib/Home.svelte"
    import Body from "../lib/Body.svelte"
    import SideBySide from "../lib/SideBySide.svelte"
    import headshot from "../assets/headshot.png"
    import DescLink from "../lib/DescLink.svelte"
    import Card from "../lib/Cards/Card.svelte"
    import GradRevealDetails from "../lib/Cards/GradRevealDetails.svelte"

    import gh from "../assets/github.png"
    import mail from "../assets/mail.png"
    import lin from "../assets/in.png"

</script>

<title>
    Joseph Liu
</title>

<Home/>

<Body>
    <SideBySide>
        <div slot="left" class="max-height max-width">
            <div class="headshot-wrapper-2 max-height">
                <div class="headshot-wrapper max-width">
                    <img class="headshot" src={headshot}/>
                </div>
            </div>
        </div>
        <div slot="right">
            <p class="h1">
                About Me
            </p>
            <p class="text">
                Hello! I'm Joseph Liu, a third year undergraduate student at Georgia Tech with concentrations in
                Systems/Architecture and Artificial Intelligence. I'm passionate and interested in computer systems,
                distributed & high performance computing, and machine learning.
            <p class="text">
                Through my coursework and projects I've gained lots of experience with different techniques and
                technologies. Through my systems coursework I've learned about OS design, virtualization, and many aspects
                of distributed system design such as synchronization, distributed memory and storage, and algorithms like
                MapReduce which can be used to parallelize queries to different services. I've learned a lot about AI as
                well, including machine learning, computer vision, robotics, and technologies like Jupyter, NumPy, and
                PyTorch. Through projects, I've also gained experience with web and app technologies like Node.js, React.js,
                React Native, Svelte, and more.
            <p class="text">
                In the summer of 2023, I interned as a software engineer at GEICO, where worked with the Service Enablement
                team. During my time there, I learned more about how companies take advantage of cloud computing and some
                basics with technologies like Kubernetes, Microsoft Azure, and .NET Web Services.
                I audited the company's service portfolio and began work on building a new service portfolio which would
                make it easier to keep service metadata accurate and up-to-date and have better integrations with ITSM and
                other services.
            <p class="text">
                Beyond computer science and software development, I have experience with media technologies and creative
                applications. Previously, I served as the VP of Media at Lynbrook Robotics, where I learned creative tools
                such as Adobe Photoshop, Premiere Pro, and other Creative Cloud tools. In my free time I also do
                photography, illustration, and graphic design.
            </p>
        </div>  
    </SideBySide>
</Body>

<Body>
    <div class="smol" style:height=33rem>
            <a href="/experience" style:color=white>
                <Card img={exp} height=12rem padding=0>
                    <div class=grad>
                        <div class="container">
                            <div class=h2>
                                My Experience
                            </div>
                            <div class="text">
                                Click here to view my previous work experience.
                            </div>
                        </div>
                    </div>
                </Card>
            </a>
            <a href="/projects" style:color=white>
                <Card img={proj} height=12rem padding=0>
                    <div class=grad>
                        <div class="container">
                            <div class=h2>
                                My Projects
                            </div>
                            <div class="text">
                                Click here to view my most recent development projects.
                            </div>
                        </div>
                    </div>
                </Card>
            </a>
            <a href="/cover-letter" style:color=white>
                <Card img={cover} height=12rem padding=0>
                    <div class=grad>
                        <div class="container">
                            <div class=h2>
                                Cover Letter
                            </div>
                            <div class="text">
                                Click here to view my cover letter for this position.
                            </div>
                        </div>
                    </div>
                </Card>
            </a>
    </div>

    <div class="info-grid large" style="grid-template-columns: repeat(auto-fit)">
        <a href="/experience" style:color=white>
            <GradRevealDetails img={exp} height=15rem maxHeightDelta="3rem">
                <div slot=above class="h2 popup">
                    My Experience
                </div>
                <div slot=hidden >
                    Click here to view my previous work experience.
                </div>
            </GradRevealDetails>
        </a>
        <a href="/projects" style:color=white>
            <GradRevealDetails img={proj} height=15rem maxHeightDelta="3rem">
                <div slot=above class="h2 popup">
                    My Projects
                </div>
                <div slot=hidden >
                    Click here to view my most recent development projects.
                </div>
            </GradRevealDetails>
        </a>
        <a href="/cover-letter" style:color=white>
            <GradRevealDetails img={cover} height=15rem maxHeightDelta="3rem">
                <div slot=above class="h2 popup">
                    Cover Letter
                </div>
                <div slot=hidden >
                    Click here to view my cover letter for this position.
                </div>
            </GradRevealDetails>
        </a>
    </div>
    <div style:margin=4rem/>
</Body>

<Body background="#224466">
    <p class=h2>Useful Links</p>
    <div class="grid-wrapper">
        <div class="grid" style="grid-template-columns: repeat(auto-fill, minmax(20rem, 1fr))">
            <DescLink img={mail} name="E-Mail" href={"mailto:jliu955+site@gatech.edu"} width=20rem>
                If you want to get touch in me, the best way to do so is through e-mail. Don't hesitate 
                to send me a message!
            </DescLink>
            <DescLink img={lin} name="LinkedIn" href={"https://linkedin.com/in/josephliu24"} width=20rem>
                Click the link below to access my LinkedIn profile. Feel free to send me a connection request!
            </DescLink>
            <DescLink img={gh} name="GitHub" href={"https://google.com"} width=20rem>
                GitHub is where I store all my code for my personal development work. 
            </DescLink>
        </div>
    </div>
    <div style:margin-bottom=2rem/>
</Body>

<style>

    .headshot-wrapper {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-right: 2rem;
    }

    .headshot-wrapper-2 {
        display: flex;
        align-items: center;
    }

    .headshot {
        width: 100%;
        max-width: 500px;
        margin: 2rem;
    }

    .grid-wrapper {
        display: flex;
        flex-direction: column;
        align-items: center;
    }    

    .grid {
        display: grid;
        grid-gap: 3rem;
        align-self: stretch;
    }

    .info-grid {
        display: grid;
        grid-column-gap: 1rem;
        grid-template-columns: 1fr 1fr 1fr;
    }

    .smol {
        display: none;
    }

    .grad {
        width: 100%;
        height: 100%;
        background: linear-gradient(transparent 20%, #000000ee);
        position: relative;
    }

    .container {
        padding: 1.5rem;
        position: absolute;
        bottom: 0;
    }

    @media(max-width: 1150px) {
        .popup {
            font-size: 2rem;
        }
    }

    @media(max-width: 900px) {
        .info-grid {
            display: grid;
            grid-template-columns: 1fr;
            row-gap: 1rem;
        }
    }

    @media(max-device-width: 900px) {
        .large {
            display: none;
        }

        .smol {
            display: flex;
            gap: 1rem;
            flex-direction: column;
        }
    }

    @media(max-width: 825px) {
        .headshot {
            max-width: 250px;
        }
    }

    @media(max-width: 700px) {
        .headshot {
            margin-bottom: 0;
            margin-top: 4rem;
        }
    }

</style>