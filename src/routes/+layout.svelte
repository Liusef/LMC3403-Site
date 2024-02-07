<script>
    import '../app.css'
    import Header from "$lib/header/Header.svelte";
    import Footer from "$lib/footer/Footer.svelte";
    import PageTransition from '../lib/PageTransition.svelte';
    import {page} from '$app/stores'
</script>

<header>
    <Header/>
</header>

<main >
    <PageTransition update={$page.data}>
        <slot/>
    </PageTransition>
</main>

<footer>
    <Footer/>
</footer>
