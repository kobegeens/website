<script>
    import Footer from "$lib/components/Footer.svelte"
    import "/src/app.css"
</script>

<svelte:head>
    <title>Kobe Geens</title>
</svelte:head>

<nav>
	<a href="/">home</a>
	<a href="/">about</a>
</nav>

<main> 
    <slot />
</main>

<Footer />