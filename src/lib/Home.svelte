<script>
    import bg from '../assets/title.jpg'
    import PageTransition from './PageTransition.svelte';
    import Socials from "./Socials.svelte";
    import { page } from '$app/stores'
    import {fade} from "svelte/transition";
</script>



<div class="home-out" id="home" style:background-image={`url(${bg})`}>
    <div class="row-center max-height center-text relative" style:z-index="1">
        <PageTransition url={$page.url.pathname}>
            <div class="title" in:fade|global>
                <p class="h1 half-ls">
                    I'm Joseph
                <p class="text half-ls">
                    I'm an undergraduate studying Computer Science at the Georgia Institute of Technology.
                </p>
            </div>
        </PageTransition>
        <!-- <div class="social-spot">
            <Socials/>
        </div> -->
    </div>
    
</div>



<style>

    .home-out {

        height: 100vh;
        width: 100%;
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        background-attachment: fixed;
        /* background: none; */
    }

    .center-text {
        width: 80vw;
        margin-left: 8vw;
        margin-right: 2rem;
    }

    .social-spot {
        position: absolute;
        bottom: 10vh;
    }

    @keyframes float {
        0% {
            transform: translate3d(0, 50px, 0);
            opacity: 0;
        }
        60% {
            opacity: 100%;
        }
        100% {
            transform: translate3d(0, 0, 0);
        }
    }

    .title {
        animation: 0.5s cubic-bezier(0, 0.5, 0.5, 1) float;
        max-width: calc(100vw - 2 * var(--title-pad-h));
        overflow-x: hidden;
    }

</style>
