<script>
import { page } from "$app/state";
import { base } from "$app/paths";
import { Nav } from "$lib/data/nav";

import radauTextLogo from "$lib/images/radau-logo-text-only.svg";
</script>

<header class="top-0 lg:sticky pt-2 bg-gray-300">
    <nav>
        <ul class="flex text-2xl font-semibold">
            {#each Nav as item, index}
                {#if index === 0}
                    <li class="flex-grow">
                        <a
                            class:active={page.route.id === item.path}
                            href={item.path}
                        >
                            <img
                                src={radauTextLogo}
                                alt="Radau logo home button"
                                class="w-24 duration-200 hover:scale-110"
                            />
                        </a>
                    </li>
                {:else}
                    <li>
                        <a
                            class:active={page.route.id === item.path}
                            href="{base}{item.path}">{item.title}</a
                        >
                    </li>
                {/if}
            {/each}
        </ul>
    </nav>
</header>

<style>
li {
    padding: 0 0.5rem;
}

.active {
    text-decoration: underline;
}
</style>
