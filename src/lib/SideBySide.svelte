<script>
    export let reverse = false
    export let leftZ = 0
    export let rightZ = 0
    export let gap = "1rem"
</script>

<div class="grid" style={`--sxs-mobile-left-row: ${reverse?2:1}; --sxs-mobile-right-row: ${reverse?1:2}; --sxs-grid-gap: ${gap};`}>
    <div class="grid-left max-width max-height" style:z-index={leftZ}>
        <slot name="left"/>
    </div>
    <div class="grid-right max-width max-height" style:z-index={rightZ}>
        <slot name="right"/>
    </div>
</div>

<style>

    .grid {
        display: grid;
        grid-column-gap: var(--sxs-grid-gap);
        grid-template-columns: 1fr 1fr;
        place-items: center;
    }

    .grid-left {
        grid-column: 1;
    }

    .grid-right {
        grid-column: 2;
    }

    @media (max-width: 700px) {
        .grid {
            grid-template-columns: 1fr;
            grid-row-gap: 2rem;
        }

        .grid-left {
            grid-row: var(--sxs-mobile-left-row);
        }

        .grid-right {
            grid-row: var(--sxs-mobile-right-row);
            grid-column: 1;
        }
    }

</style>