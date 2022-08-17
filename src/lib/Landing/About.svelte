<script>
    import LayoutGrid, {Cell} from "@smui/layout-grid";

    export let about = {}

</script>
<section class='bg'>
    <LayoutGrid style='padding: 0; min-height: 500px;'>
        <Cell span='6'>
            <div class="img-about">
                <img src="{about.image}">
            </div>
        </Cell>
        <Cell span='6'>
            <LayoutGrid>
                <Cell span='8' style='text-align: left'>
                    <p class="green-color font-ligth" style='text-align: left'>ABOUT</p>

                    <h2 class="font-cinzel">{about.title}</h2>
                    <p class="font-regular" style='text-align: left'>{about.description}</p>
                </Cell>
            </LayoutGrid>

        </Cell>
    </LayoutGrid>
</section>
<style>
    .bg {
        background: white;
    }

</style>
