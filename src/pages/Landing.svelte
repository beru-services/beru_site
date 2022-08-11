<script>
    import Header from "../lib/Landing/Header.svelte";
    import About from "../lib/Landing/About.svelte";
    import Services from "../lib/Landing/Services.svelte";
    import OurWork from "../lib/Landing/OurWork.svelte";
    import AboutTwo from "../lib/Landing/AboutTwo.svelte";
    import Footer from "../lib/Landing/Footer.svelte";

    console.log(import.meta.env.VITE_SOME_KEY)
</script>

<Header />

<About />

<Services />

<OurWork />

<AboutTwo />

<Footer />

<style>
    @import "../assets/css/landing.css";
</style>
