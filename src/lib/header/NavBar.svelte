<script>
    import NavLink from "./NavLink.svelte"
    import {base} from "$app/paths"
</script>


<div class="flex-out">

    <NavLink href="{base}/">
        ABOUT
    </NavLink>
    <NavLink href="{base}/experience">
        EXPERIENCE
    </NavLink>
    <NavLink href="{base}/projects">
        PROJECTS
    </NavLink>
    <NavLink href="{base}/cover-letter">
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
