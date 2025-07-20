<script>
    import Footer from "$lib/components/Footer.svelte";
    import "$lib/assets/app.css"
</script>

<svelte:head>
    <title>Kobe Geens</title>
</svelte:head>

<nav style="background-color: var(--backgroundcolor2); border-radius: 30px; padding: 1em;">
    <a style="margin:auto">Home</a> <a style="margin:auto">Projects</a> <a style="margin:auto">About me</a>
</nav>

<main> 
    <slot />
</main>

<Footer />