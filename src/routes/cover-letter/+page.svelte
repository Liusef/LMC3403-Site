<script>

    import img from "../../assets/cover.jpg"
    import Title from "$lib/Title.svelte"
    import Body from "../../lib/Body.svelte";

</script>


<Title {img} title="Cover Letter">
    <div class=large-text style:margin-top=1.5rem>
        My cover letter for this position.
    </div>
</Title>

<Body>
    <div class="col-center">
        <div style:max-width=800px>
            <p>
                Dear Amazon Web Services Recruiting Team,
            </p>
            <p>
                I&rsquo;m writing to apply for a software engineering position with Amazon Web Services. 
                Amazon Web Services (AWS) is a leader in the cloud services industry, not only in numbers, 
                but also in quality of your services. As a computer science major at Georgia Tech with concentrations 
                in artificial intelligence and computer systems/architecture, I would love an opportunity to work on a 
                service that allows so many developers to transform their visions into reality. &nbsp;
            </p>
            <p>
                Through some of my recent projects and coursework, I&rsquo;ve gotten exposure to both AWS and cloud 
                computing technology in general. During my most recent internship, I got to see how companies use cloud 
                computing technology to save costs and improve the customer experience. I also got to use AWS&rsquo;s 
                tooling myself on one of my recent projects, which I instantly fell in love with.
            </p>
            <p>
                My experience has also prepared me to work on cloud computing systems. I&rsquo;ve taken many courses on low l
                evel systems, like processor design, operating systems, OS design, distributed systems, and system design for 
                cloud computing. Additionally, I have experience working with applications running on the cloud, like 
                different projects that I&rsquo;ve written that utilize services like Amazon&rsquo;s EC2 and DynamoDB.
            </p>
            <p>
                I greatly appreciate this opportunity to contribute to Amazon Web Services and I hope to hear back from 
                you or your team soon. Thank you so much for your time and consideration.
            </p>
            
            <p>Sincerely,</p>
            <p>Joseph Liu</p>
        </div>
    </div>
</Body>

<style>
    p {
        font-size: 1.25rem;
    }
</style>
