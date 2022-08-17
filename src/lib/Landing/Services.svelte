<script>
    import {Cell} from "@smui/layout-grid";
    import {beforeUpdate} from "svelte";

    let image = new URL('../../assets/images/Rectangle11.png', import.meta.url).href;
    let image_decoration  = new URL('../../assets/images/icon.png', import.meta.url).href;

    export let service = {}
    let title
    let subtitleOne
    let subtitleTwo

    beforeUpdate(async function() {
        if (service.title) {
            title = service.title.substring(0, service.title.lastIndexOf(' '))
            subtitleOne = title.substring(title.lastIndexOf(' '))

            title = title.replace(subtitleOne, '')
            subtitleTwo = service.title.substring(service.title.lastIndexOf(' '))
        }


    })

</script>
<section class="services">
    <h1 class="font-cinzel white-color">
        {#if title}
        {title}
        <span class="green-color">{subtitleOne} {subtitleTwo}</span>
        {/if}
    </h1>
    <img src="{image_decoration}" style = "margin-top: 10px">

    <div class="container-center">
        {#if service.service}
            {#each service.service as service}
                <Cell span="2" style="margin-left: 4px; margin-right: 4px;">
                    <div class="container-image">
                        <h2 class="title">{service.title}</h2>
                        <img src="{image}">
                        <div class="detail-service">
                            <h2>{service.title}</h2>

                            <p class="font-regular">
                                {service.description}
                            </p>
                        </div>
                    </div>

                </Cell>
            {/each}
        {/if}
    </div>
</section>

<style>
    .title {
        margin-top: 3rem; position: absolute
    }
    .container-center {
        display: flex;
        justify-content: center;
        align-content: center;
        width: 100%;
        margin-top: 3rem;
        height: 300px;
    }

    .services {
        padding: 6rem 2rem 2rem 4rem;
    }

    .container-image img{
        height: 224px;
        width: 100%;
    }

    .container-image {
        position: relative;
        overflow: hidden;
        height: 159px;
        width: 100%;
        transition-duration: 1s, 0s;
    }

    .detail-service {
        position: absolute;
        height: 100%;
        width: 100%;
        background: rgba(42, 36, 39, .3);
        top: 0;
        z-index: 1;
        padding: 4px;
        overflow: hidden;
        transition-duration: 1s, 0s;
        opacity: 0;
    }

    h2 {
        font-size: 1.4rem;
        color: white;
        z-index: 1;
    }

    .detail-service > p{
        color: white;
    }

    .container-image:hover {
        height: 220px;
        border-left: #7FB61E 4px solid;

    }

    .container-image:hover .detail-service {
        opacity: 1;
    }

    .container-image:hover .title {
        display: none;
    }


    /*.container-image img{*/
    /*    position: absolute;*/
    /*}*/
</style>
