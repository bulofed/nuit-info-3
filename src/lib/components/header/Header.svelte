<!-- Header.svelte -->
<header>
    <NavBar>
        <MenuButton slot="menu-button" {isMenuOpen} {toggleMenu} />
        <MenuItems slot="menu-items" {isMenuOpen} />
    </NavBar>
</header>

<script>
    import NavBar from './NavBar.svelte';
    import MenuButton from './MenuButton.svelte';
    import MenuItems from './MenuItems.svelte';

    let isMenuOpen = false;

    function toggleMenu() {
        isMenuOpen = !isMenuOpen;
    }
</script>