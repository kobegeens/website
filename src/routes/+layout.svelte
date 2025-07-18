<script>
	let { children } = $props();
    import "/src/app.css"
</script>

<nav>
	<a href="#">home</a>
	<a href="#">about</a>
</nav>

<main> 
    {@render children()}
</main>

<footer>
    <p>Copyright (c) 2025 Kobe Geens</p>
</footer>