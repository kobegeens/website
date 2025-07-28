<script>
    import questionmark from '$lib/assets/questionmark.png';
    import kobesterminal from '$lib/assets/kobesterminal.png';
</script>

<style>
.gridcontainer {
    display: grid; 
    grid-template-columns: repeat(auto-fit,  minmax(20em, 1fr));
}

a, a:active, a:visited, a:hover {
    text-decoration: none;
    color: var(--textcolor);
}
.griditem {
    width: inherit;
    background-color: var(--backgroundcolor2);
    border-radius: 30px;
    margin: 0.5em;
    display: flex;
    flex-direction: row;
    opacity: 75%;
    padding: 0.5em;
}
.griditem:hover {
    opacity: 100%;
    transform: scale(1.05);
}
img {
    display: block;
    width: 7.5em;
    aspect-ratio: 1 / 1;
    object-fit: contain;
    border-radius: 15px;
    margin: 0.5em;
}
</style>

<div class="gridcontainer">
    <a href="https://kobegeens.neocities.org">
        <div class="griditem">
            <img src="{kobesterminal}" alt="project"/>
            <div>
                <h2>Kobe's terminal</h2>
                <p>
                    A stylised personal-website.
                    <br>
                    <small>
                        HTML/CSS
                        <br>
                        2023
                    </small>
                </p>
            </div>
        </div>
    </a>
    <div class="griditem">
        <p>Project1</p>
        <img src="{questionmark}" alt="project"/>
    </div>
</div>