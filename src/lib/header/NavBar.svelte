<script>
    import NavLink from "./NavLink.svelte"
</script>


<div class="flex-out">

    <NavLink href="/">
        ABOUT
    </NavLink>
    <NavLink href="/experience">
        EXPERIENCE
    </NavLink>
    <NavLink href="/projects">
        PROJECTS
    </NavLink>
    <NavLink href="/cover-letter">
        COVER LETTER
    </NavLink>

</div>


<style>
    .flex-out {
        display: flex;
        flex-direction: row;
        gap: 2rem;
        align-items: center;
    }
</style>
