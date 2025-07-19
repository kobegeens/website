<script>
    import Footer from "$lib/components/Footer.svelte";
</script>

<svelte:head>
    <title>Kobe Geens</title>
</svelte:head>

<nav style="background-color: var(--backgroundcolor2); border-radius: 30px; padding: 1em;">
    <p>Home     Projects     About me</p>
</nav>

<main> 
    <slot />
</main>

<Footer />