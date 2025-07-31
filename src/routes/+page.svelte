<script lang="ts">
    import pfp from '$lib/assets/pfp.png';
    import { onMount } from 'svelte';
    import Projects from '$lib/components/Projects/Projects.svelte';

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

<h3>About Me</h3>
<p>Hey, I'm Kobe! I'm a student from 2008 interested in both software and hardware engineering. You might know me from programs I participate in such as Hack Club.</p> 
<p>If you wish to contact me feel free to do so via <a href="mailto:kobegeens@proton.me">e-mail</a>!</p>

<hr>

<h3>Main Projects</h3>
<Projects />
<a href="projects">view more</a>

<hr>

<h3>Why?</h3>
<p>This site was created for the Smelt YSWS from Hack Club. It will mostly be used to centralise and parade with my projects.</p>

<hr>


<h3>To Do</h3>
<ul>
    <li>lucide icons</li>
    <li>animations</li>
    <li>photo viewer</li>
</ul>

<hr>


