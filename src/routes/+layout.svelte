<script>
import Header from "./Header.svelte";
import Footer from "./Footer.svelte";
import "./styles.css";
</script>

<div class="bg-gray-300 w-full max-w-full overflow-x-hidden">
    <Header />
    <main class="mx-[10%] xl:mx-[30%] min-h-screen">
        <slot />
    </main>
    <Footer />
</div>
