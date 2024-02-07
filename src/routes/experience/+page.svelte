<script>

    import img from "../../assets/exp.jpg"
    import Title from "$lib/Title.svelte"
    import Body from "../../lib/Body.svelte";
    import Divider from "../../lib/Divider.svelte"
    import SideBySide from "../../lib/SideBySide.svelte";
    import Card from "../../lib/Cards/Card.svelte";
    import HoverCard from "../../lib/Cards/HoverCard.svelte";

</script>


<Title {img} title="Experience">
    <div class="large-text" style:margin-top=1.5rem>
        My previous work experience.
    </div>
</Title>

<div style:margin=6rem/>

<Body>
    <HoverCard background="linear-gradient(120deg, #096C6E, #021A14 )" overlayBackground="linear-gradient(120deg, #028A89, #024A59)">
        <div style:margin=1.5rem/>
        <SideBySide gap="3rem">
            <div slot=left class=left-container>
                <div class="h1 titles">GEICO Tech</div>
                <div class=h4 style:margin-top=0.5rem>Software Engineering Intern (TDP)</div>
                <div class=text>Chevy Chase, MD</div>
                <div class=text>June 2023 - August 2023</div>
            </div>
            <div slot=right class=right-container>
                <ul>
                    <li><p>Audited and corrected over 150 items in the company’s service portfolio to ensure accurate service metadata</li>
                    <li><p>Reverse engineered an authentication scheme for an old GEICO service with little to no documentation to automate notification of teams in case of critical service issues</li>
                    <li><p>Pioneered and led an initiative to build a new IT service portfolio to streamline the process of onboarding, modifying, and certifying services and their respective metadata using ASP.NET Core and Azure Kubernetes Services</li>
    
                </ul>
            </div>
        </SideBySide>
    </HoverCard>
</Body>


<Body>
    <HoverCard background="linear-gradient(120deg, #093C6E, #020A14 )" overlayBackground="linear-gradient(120deg, #025A89, #022A59)">
        <div style:margin=1.5rem/>
        <SideBySide gap="3rem">
            <div slot=left class=left-container>
                <div class="h1 titles">Empathy Bytes</div>
                <div class=h4 style:margin-top=0.5rem>Student Researcher and Developer</div>
                <div class=text>Atlanta, GA</div>
                <div class=text>August 2021 - December 2022</div>
            </div>
            <div slot=right class=right-container>
                <ul>
                    <li><p>Spearheaded a team that built an augmented reality application using <strong>Unity</strong> and <strong>ARFoundation</strong> that allows users to explore The Hive makerspace from any mobile device to increase accessibility and immersion</li>
                    <li><p>Created a mobile app using <strong>React Native</strong>, <strong>js</strong>, <strong>RESTful APIs</strong>, and <strong>GraphQL</strong> that lets users browse Empathy Bytes&rsquo; archive of resources to make our app cross platform and reduce work needed to maintain our mobile app</li>
                    <li><p>Established a team that created an interactive VR experience using <strong>Unity</strong> and <strong>OpenXR</strong> so people can view and interact with different artifacts from the Georgia Tech Archives</li>
                </ul>
            </div>
        </SideBySide>
    </HoverCard>
</Body>

<Body>
    <HoverCard background="linear-gradient(120deg, #6E0C09, #140A02 )" overlayBackground="linear-gradient(120deg, #820A09, #490A02)">
        <div style:margin=1.5rem/>
        <SideBySide gap="3rem">
            <div slot=left class=left-container>
                <div class="h2 titles">Mathnasium</div>
                <div class=h4 style:margin-top=0.5rem>Mathematics Instructor</div>
                <div class=text>Mountain View, CA</div>
                <div class=text>May 2022 - August 2022</div>
            </div>
            <div slot=right class=right-container>
                <ul>
                    <li><p>Taught students a variety of fields of mathematics, from addition and subtraction to university calculus</li>
                    <li><p>Oversaw and personally instructed multiple students at any given time</li>
                </ul>
            </div>
        </SideBySide>
    </HoverCard>
</Body>



<style>
    .left-container {
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: flex-end;
        text-align: right;
    }

    .titles {
        margin-top: 1.5rem;
    }

    p {
        font-size: 1.25rem;
    }

    ul {
        max-width: 600px;
    }

    @media(max-width:825px) {
        .titles {
            font-size: 3rem;
        }

        li {
            margin-left: -2rem;
        }
    }

    @media(max-width:700px) {
        .left-container {
            align-items: flex-start;
            text-align: left;
        }

        .titles {
            margin-top: 0;
        }

        li {
            margin-left: -1rem;
        }
    }

</style>