<script>
    export let isMenuOpen;
    const menuItems = [
        { href: "/jeu", text: "Jeu" },
        { href: "/", text: "Prévention" }
    ];
</script>

<div class={`justify-between items-center w-full lg:flex lg:w-auto ${isMenuOpen ? 'flex' : 'hidden'}`} id="mobile-menu-2">
    <ul class="flex flex-col mt-4 font-medium lg:flex-row lg:space-x-8 lg:mt-0 w-full">
        {#each menuItems as item}
            <li>
                <a href={item.href} class="block py-2 pr-4 pl-3 text-zinc-700 border-b border-zinc-100 hover:bg-zinc-50 lg:hover:bg-transparent lg:border-0 lg:hover:text-primary-700 lg:p-0 dark:text-zinc-400 lg:dark:hover:text-white dark:hover:bg-zinc-700 dark:hover:text-white lg:dark:hover:bg-transparent dark:border-zinc-700 font-medium">{item.text}</a>
            </li>
        {/each}
    </ul>
</div>