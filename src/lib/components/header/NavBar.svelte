<nav class="bg-white border-zinc-200 px-4 lg:px-6 py-2.5 dark:bg-zinc-800">
    <div class="flex flex-wrap justify-between items-center mx-auto max-w-screen-xl">
        <a href="/" class="flex items-center">
            <span class="self-center text-xl font-semibold whitespace-nowrap dark:text-white">Logo</span>
        </a>
        <slot name="menu-button"></slot>
        <slot name="menu-items"></slot>
    </div>
</nav>