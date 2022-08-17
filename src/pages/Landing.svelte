<script>
    import { onMount } from "svelte";
    import Header from "../lib/Landing/Header.svelte";
    import About from "../lib/Landing/About.svelte";
    import Services from "../lib/Landing/Services.svelte";
    import OurWork from "../lib/Landing/OurWork.svelte";
    import AboutTwo from "../lib/Landing/AboutTwo.svelte";
    import Footer from "../lib/Landing/Footer.svelte";
    import Loading from "../lib/Components/Loading.svelte";

    let aboutFirstSection
    let aboutSecondSection
    let services
    let gallery
    let header
    let request = true
    const URL_API = import.meta.env.VITE_URL_API + "v1/web/site"
    const TOKEN_API = import.meta.env.VITE_TOKEN_API


    onMount(async function() {
        console.log(URL_API.trim() )

        const response = await fetch(URL_API.replace('"', ''), {
            method: 'GET',
            headers: {
                'Authorization': "Bearer " + TOKEN_API.trim(),
            },
        })

        const dataResponse = await response.json()

        aboutFirstSection = dataResponse.about_first_section[0]

        aboutSecondSection = dataResponse.about_second_section[0]

        services = dataResponse.services[0]

        gallery = dataResponse.gallery.gallery_image

        header = dataResponse.header


        setTimeout(() => {
            request = false
        },300)
    })


</script>

{#if !request}
    <Header data={header} />

    <About about={aboutFirstSection} />

    <Services service={services} />

    <OurWork images={gallery} />

    <AboutTwo about={aboutSecondSection} />

    <Footer />
{:else}
    <Loading />
{/if}

<style>
    @import "../assets/css/landing.css";
</style>
