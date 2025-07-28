<script>
    import Footer from "$lib/components/Footer.svelte";
    import Navbar from "$lib/components/Navbar.svelte";
    import "$lib/assets/app.css"
</script>

<Navbar />

<svelte:head>
    <title>𝗞𝗼𝗯𝗲 𝗚𝗲𝗲𝗻𝘀</title>
</svelte:head>



<main> 
    <slot />
</main>
<Footer />