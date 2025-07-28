<script lang="ts">
    import pfp from '$lib/assets/pfp.png';
    import { onMount } from 'svelte';
    import Projects from '$lib/components/Projects.svelte';

      let repos = [];

  onMount(async () => {
    const res = await fetch('https://api.github.com/users/kobegeens/repos');
    repos = await res.json();
  });
</script>

<div style="display: flex; flex-direction: column; align-items:center;">
    <img src="{pfp}" alt="profile picture" style="width:10em; margin:0.5em; border-radius:50%; border-style:solid;">
    <h1>Kobe Geens</h1>
    <p>パリに行けないなら、神戸に行け。</p>
</div>

<hr>

<div style="text-align: center;">
    <b>
        <h3>
            <a href="https://glennm008.github.io/website/">&lt;----</a> Hack Club Heist <a href="https://jackhaesen.github.io/personal-website/">----&gt;</a>
        </h3>
    </b>
</div>
<hr>

<h3>About Me</h3>
<p>Hey, I'm Kobe! I'm a student from 2008 interested in both software and hardware engineering. You might know me from programs I participate in such as Hack Club.</p> 
<p>If you wish to contact me feel free to do so via <a href="mailto:kobegeens@proton.me">e-mail</a>!</p>

<hr>

<h3>Main Projects</h3>
<Projects />
<a>view more</a>

<hr>

