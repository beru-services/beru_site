<script>
    import LayoutGrid, {Cell} from "@smui/layout-grid";
</script>
<section class='bg'>
    <LayoutGrid style = 'padding: 0; min-height: 500px;'>
        <Cell span='6'>
            <div class="img-about"></div>
        </Cell>
        <Cell span='6'>
            <LayoutGrid>
                <Cell span = '8' style = 'text-align: left'>
                    <p class="green-color font-ligth" style = 'text-align: left'>ABOUT</p>
                    <h2 class="font-cinzel">BEST LAUNDRY SERVICE FOR YOUR JET</h2>

                    <p class="font-regular" style = 'text-align: left'>Lorem ostrud amet.Amet minim mollit non deserunt ullamco est sit aliqua dolor do amet sint. Velit officia
                        consequat duis enim velit mollit. Exercitation veniam consequat sunt nostrud amet.Amet minim mollit non
                        deserunt ullamco est sit aliqua dolor do amet sint. Velit officia consequat duis enim velit mollit.
                        Exercitation veniam consequat sunt nostrud amet.Amet minim mollit non deserunt ullamco est sit aliqua
                        dolor do amet sint. Velit officia consequat duis enim velit mollit.</p>
                </Cell>
            </LayoutGrid>

        </Cell>
    </LayoutGrid>
</section>
<style>
    .bg {
        background: white;

    }

    .img-about {
        min-height: 500px;
        background-size: cover;
        background: url("../../assets/images/bg-about.png") no-repeat;
        width: 100%;
        height: 100%;
    }

</style>
