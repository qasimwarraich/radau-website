<script>
import About from "./About.svelte";
import Hero from "./Hero.svelte";
import Map from "./Map.svelte";
</script>

<svelte:head>
    <title>Rad.au</title>
    <meta name="description" content="Rad.au Homepage" />
</svelte:head>

<section class="flex flex-col items-center justify-center gap-y-3 mb-2">
    <Hero />
    <About />
    <Map />
</section>
