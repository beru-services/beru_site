<script>

    import Carousel from "../Components/Carousel.svelte";

    let image_decoration  = new URL('../../assets/images/icon.png', import.meta.url).href;

    export let images = [];
</script>

<div class="section-gallery">
    <h2 class="font-cinzel">Our <span class="green-color">Work</span></h2>
    <img src="{image_decoration}" style = "margin-top: 10px; margin-bottom: 2rem">
    <Carousel
            {images}
            imageWidth={250}
            imageSpacing={15}
            controlScale={0.8}
            displayControls={true}
            autoplay={false}
            autoplaySpeed={3000}
    />


</div>


<style>
    .section-gallery {
        background: url("src/assets/images/bg-works.png") white;
        background-repeat: no-repeat;
        background-position: right;
        padding: 3rem;
    }
</style>
