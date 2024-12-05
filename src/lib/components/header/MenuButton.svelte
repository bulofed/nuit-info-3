<script>
    export let isMenuOpen;
    export let toggleMenu;

    import BurgerMenu from '$lib/icons/BurgerMenu.svelte';
    import XMenu from '$lib/icons/XMenu.svelte';
</script>

<button on:click={toggleMenu} type="button" class="inline-flex items-center p-2 ml-1 rounded-lg lg:hidden hover:bg-zinc-100 focus:outline-none focus:ring-2 focus:ring-zinc-200 dark:hover:bg-zinc-700 dark:focus:ring-zinc-600" aria-controls="mobile-menu-2" aria-expanded={isMenuOpen}>
    <span class="sr-only">Ouvrir le menu</span>
    <BurgerMenu {isMenuOpen} />
    <XMenu {isMenuOpen} />
</button>