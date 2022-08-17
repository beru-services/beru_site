<script>
    import LayoutGrid, {Cell} from "@smui/layout-grid";

    export let about = {}
</script>

<section class="container-main">
    <LayoutGrid style='padding: 0;'>
        <Cell span='6' style="text-align: left">
            <p class="green-color font-ligth" style='text-align: left'>ABOUT</p>
            <h2 class="font-cinzel white-color">{about.title}</h2>

            <p class="font-regular white-color" style='text-align: left'>{about.description}</p>

        </Cell>
        <Cell span='6'>
            <div class="img-about">
                <img src="{about.image}">
            </div>

        </Cell>
    </LayoutGrid>
</section>
