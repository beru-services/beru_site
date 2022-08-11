<script>
    import LayoutGrid, {Cell} from "@smui/layout-grid";
</script>

<section class="container-main">
    <LayoutGrid style='padding: 0;'>
        <Cell span='6' style="text-align: left">
            <p class="green-color font-ligth" style='text-align: left'>ABOUT</p>
            <h2 class="font-cinzel white-color">AREAS WE SERVE</h2>

            <p class="font-regular white-color" style='text-align: left'>Lorem ostrud amet.Amet minim mollit non
                deserunt ullamco est sit aliqua dolor do amet sint. Velit officia
                consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.Amet minim mollit non
                deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit.
                Exercitation veniam consequat sunt nostrud amet.Amet minim mollit non deserunt ullamco est sit aliqua
                dolor do amet sint. Velit officia consequat duis enim velit mollit.</p>
            
        </Cell>
        <Cell span='6'>
            <div class="img-about"></div>

        </Cell>
    </LayoutGrid>
</section>
<style>

    .img-about {
        background-size: cover;
        background: url("src/assets/images/bg-about.png") no-repeat;
        width: 100%;
        height: 100%;
    }

</style>
