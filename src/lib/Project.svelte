<script>
    import Title from "$lib/Title.svelte"
    import Body from "./Body.svelte";
    import Divider from "./Divider.svelte"
    import SideBySide from "./SideBySide.svelte";
    import Card from "./Cards/Card.svelte";

    export let img
    export let title

</script>

<Body>
    <div class=col-center>
        <div style:max-width=1400px>
            <SideBySide>
                <div slot=left class="col-center" >
                    <div style:max-width=600px>
                        <div class=h2 style:margin-bottom=2rem>
                            {title}
                        </div>
                        <slot/>
                    </div>
                </div>
                <div slot=right style:height=100%>
                    <div class="col-center max-height">
                        <div class="row-center max-height">
                            <img src={img}/>
                        </div>
                    </div>
                </div>
            </SideBySide>
        </div>
        <div style:margin=3rem/>
        <Divider/>
    </div>
</Body>

<style>
    img {
        border-radius: 32px;
        max-width: 40vw;
    }

    @media(max-width: 700px) {
        img {
            max-width: 100%;
        }
    }
</style>