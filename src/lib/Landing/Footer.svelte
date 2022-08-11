<script>
    import LayoutGrid, {Cell} from "@smui/layout-grid";
    import Button, {Label} from "@smui/button";

    let src = '/src/assets/images/beru-logo.png';

    let facebook = '/src/assets/images/facebook.png';
    let tw = '/src/assets/images/twitter.png';
    let instagram = '/src/assets/images/instagram.png';
    let logo = '/src/assets/images/beru-logo.png';
</script>
<div class="line"></div>
<footer class="container-main">
    <LayoutGrid>
        <Cell span='10'>
            <LayoutGrid style="padding: 0">
                <Cell span="4">
                    <a href="#/" class="logo">
                        <img src="{logo}">
                    </a>
                </Cell>
                <Cell span="2" style="padding-top: 2rem;">
                    <a href="">
                        SERVICE
                    </a>
                </Cell>
                <Cell span="2" style="padding-top: 2rem;">
                    <a href="">
                        ABOUT
                    </a>
                </Cell>
                <Cell span="2" style="padding-top: 2rem;">
                    <a href="">
                        WE SERVICE
                    </a>
                </Cell>
                <Cell span="2" style="padding-top: 2rem;">
                    <a href="">
                        CONTACT
                    </a>
                </Cell>
            </LayoutGrid>
        </Cell>

        <Cell span='2'>
            <LayoutGrid>
                <Cell span="2" style="padding-top: 8px;">
                    <a href="#" target="_blank">
                        <img src="{facebook}"/>
                    </a>
                </Cell>
                <Cell span="2" style="padding-top: 8px;">
                    <a href="#" target="_blank">
                        <img src="{tw}"/>
                    </a>
                </Cell>
                <Cell span="2" style="padding-top: 8px;">
                    <a href="#" target="_blank">
                        <img src="{instagram}"/>
                    </a>
                </Cell>
                <Cell span="6">
                </Cell>
            </LayoutGrid>
        </Cell>
    </LayoutGrid>

</footer>

<style>
    .line {
        border-top: 1px solid #7FB61E;
        margin-top: 3rem;
    }
</style>
