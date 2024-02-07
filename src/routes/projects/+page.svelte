<script>

    import img from "../../assets/projects.jpg"
    import Title from "$lib/Title.svelte"
    import Body from "../../lib/Body.svelte";
    import Divider from "../../lib/Divider.svelte"
    import SideBySide from "../../lib/SideBySide.svelte";
    import Card from "../../lib/Cards/Card.svelte";
    import Project from "../../lib/Project.svelte";

    import mr from "../../assets/proj/mapreduce.png"
    import ba from "../../assets/proj/barrier.png"
    import gba from "../../assets/proj/gba.png"
    import gitlet from "../../assets/proj/gitlet.png"
    import maze from "../../assets/proj/maze.png"
    import ml from "../../assets/proj/meetinglauncher.png"
    import nn from "../../assets/proj/nn.png"
    import stats from "../../assets/proj/stats.png"
    import tg from "../../assets/proj/tgstickers.png"
    import zoom from "../../assets/proj/zoom.png"
    
</script>


<Title {img} title="Projects">
    <p class=large-text>
        My recent development projects.
    </p>
</Title>

<Project img={mr} title="MapReduce">
    <ul>
        <li>Implemented the MapReduce framework which can parallelize compute processing of colossal datasets between tens of thousands of machines, such as processing web search results in a datacenter</li>
        <li>Utilized <strong>gRPC</strong> to support high speed and reliable communication between remote computers and <strong>pthreads</strong> to parallelize and synchronize work done on individual machines in the cluster</li>
        <li>Made the program was fault tolerant by ensuring that all work is completed even if machines die or temporarily go offline</li>
    </ul>
</Project>

<Project img={ba} title="Distributed Barrier Synchronization">
    <ul>
        <li>Developed a barrier algorithm using <strong>C</strong> to synchronize threads running across many different servers in a datacenter</li>
	    <li>Leveraged industry standard <strong>OpenMP</strong> and <strong>MPI</strong> for rapid communication between different servers</li>
	    <li>Implemented the MCS tree barrier algorithm for improved performance and scalability, as well as flexibility to run efficiently on extremely large distributed systems (namely NCC-NUMA clusters)</li>

    </ul>
</Project>

<Project img={nn} title="Vectorized Neural Network">
    <ul>
        <li>Created Multilayer Perceptron Neural Network with ReLU and SoftMax layers and the SGD Optimizer for a simple implementation while preserving performance 
        <li>Wrote Neural Network using NumPy arrays and vectorized algorithms for fast execution without expensive hardware

    </ul>
</Project>

<Project img={tg} title="Telegram Sticker Pack Manager">
    <ul>
        <li>Wrote an application to automate tasks with Telegram’s sticker bot and make managing stickers simpler and less tedious
        <li>Used Telegram’s MTProto communication API to send and receive information from Telegram’s secure servers 
        <li>Utilized asynchronous programming, parallelization, intelligent caching, image processing, and unit testing to increase throughput, reduce latency, and ensure reliability

    </ul>
</Project>

<Project img={gba} title="Game Boy Advance Platformer">
    <ul>
        <li>Programmed a simple Game Boy Advance platformer game using C and provided ABIs for the Game Boy
        <li>Used Memory Mapped I/O (MMIO) to draw to the display and read user input
        <li>Took advantage special DMA hardware in the Game Boy Advance to speed up certain tasks and improve rendering quality

    </ul>
</Project>

<style>

    

    li {
        margin-bottom: 1rem;
    }

</style>


