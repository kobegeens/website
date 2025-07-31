

<style>
.gridcontainer {
    display: grid; 
    grid-template-columns: repeat(auto-fit,  minmax(10em, 1fr));
    gap: 0.5em;
    margin: 0.5em;
}

img {
    width: 100%;
    display: block;
    aspect-ratio: 1 / 1;
    object-fit: cover;
}
img:hover {
    transform: scale(1.2);
}
</style>

<!-- Automate photo insertion and create viewer.-->
<div class="gridcontainer">
    <img src="photos/jake.jpg" class="hover" alt="project" />
    <img src="photos/jake.jpg" class="hover" alt="project" />
    <img src="photos/jake.jpg" class="hover" alt="project" />
    <img src="photos/jake.jpg" class="hover" alt="project" />
    <img src="photos/jake.jpg" class="hover" alt="project" />
    <img src="photos/jake.jpg" class="hover" alt="project" />
    <img src="photos/jake.jpg" class="hover" alt="project" />
    <img src="photos/jake.jpg" class="hover" alt="project" />
    <img src="photos/jake.jpg" class="hover" alt="project" />
</div>