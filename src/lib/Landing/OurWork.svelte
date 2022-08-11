<script>

    import Carousel from "../Components/Carousel.svelte";

    let bg_img = "src/assets/images/bg-works.png";
    let image_decoration  = "src/assets/images/icon.png";

    const images = [
        {
            path: 'https://picsum.photos/id/1012/3973/2639',
            id: 'imagen-ejemplo-1',
            alt: 'Atributo ALT de ejemplo para la imagen #1',
        },
        {
            path: 'https://picsum.photos/id/1005/5760/3840',
            id: 'imagen-ejemplo-2',
            alt: 'Atributo ALT de ejemplo para la imagen #2',
        },
        {
            path: 'https://picsum.photos/id/1020/4288/2848',
            id: 'imagen-ejemplo-3',
            alt: 'Atributo ALT de ejemplo para la imagen #3',
        },
        {
            path: 'https://picsum.photos/id/1025/4951/3301',
            id: 'imagen-ejemplo-4',
            alt: 'Atributo ALT de ejemplo para la imagen #4',
        },
        {
            path: 'https://picsum.photos/id/103/2592/1936',
            id: 'imagen-ejemplo-5',
            alt: 'Atributo ALT de ejemplo para la imagen #5',
        },
        {
            path: 'https://picsum.photos/id/104/3840/2160',
            id: 'imagen-ejemplo-6',
            alt: 'Atributo ALT de ejemplo para la imagen #6',
        },
    ];
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
