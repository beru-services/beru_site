<script>
    import LayoutGrid, {Cell} from "@smui/layout-grid";
    import Button, {Label} from "@smui/button";

    const facebook = new URL('../../assets/images/facebook.png', import.meta.url).href;

    let tw = new URL('../../assets/images/twitter.png', import.meta.url).href;
    let instagram = new URL('../../assets/images/instagram.png', import.meta.url).href;
    let logo = new URL('../../assets/images/beru-logo.png', import.meta.url).href;

    export let data = {}

</script>

<header style="background-image: url('{data.image}')">
    <section class="container-main">
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
                        <Button on:click={() => hola} variant="raised" color="secondary" style="width: 100%">
                            <Label>LOGIN</Label>
                        </Button>
                    </Cell>
                </LayoutGrid>
            </Cell>
        </LayoutGrid>
    </section>
    <section class="container-main h50">
        <div class="align-center">
            <LayoutGrid align="right" style="padding: 0;"
                        fixedColumnWidth>
                <Cell align="middle" span="12" style="text-align: left">
                    <h1 class="w100 font-cinzel white-color">{data.title}</h1>
                </Cell>
                <Cell align="middle" span="12" style="text-align: left; margin-top: 10px;">
                    <h2 class="w100 font-cinzel green-color" style="line-height: 0">{data.sub_title}</h2>
                </Cell>
            </LayoutGrid>
        </div>

    </section>

</header>
