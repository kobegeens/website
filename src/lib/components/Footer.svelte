<style>
    footer {
        background-color: var(--backgroundcolor2);
        padding:1em;
        border-radius: 30px;
        text-align: center;
    }
    select {
        background-color: var(--backgroundcolor2);
        border: none;
        color: var(--textcolor);
        font-size: 1em;
    }
</style>
<footer>
    <p>Copyright (c) 
        <select id="year">
            <option value="2025">2025</option>
            <option value="1998">1998</option>
        </select>
        Kobe Geens</p>
        <a href="https://www.instagram.com/geens.kobe/">Instagram</a> <a href="">GitHub</a>
</footer>
<script lang="ts">
    import { onMount } from 'svelte';

    onMount(() => {

        const year = document.getElementById("year") as HTMLSelectElement;

        year.addEventListener("change", function () {
            if (year.value === "1998") {
                window.location.href = "https://kobegeens.neocities.org";
            }
        });
    });
</script>