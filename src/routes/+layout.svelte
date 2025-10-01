<script>
import Header from "./Header.svelte";
import Footer from "./Footer.svelte";
import "./styles.css";
</script>

<div class="bg-gray-300">
    <Header />
    <main>
        <slot />
    </main>
    <Footer />
</div>
