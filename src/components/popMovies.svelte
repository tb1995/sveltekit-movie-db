<script>

    import MovieCard from "./movieCard.svelte";
    export /**
* @type {any}
*/
     let popular;
    console.log("ALL MOVIES" , popular);
</script>

<h1>Popular movies</h1>

<div class="popularMovies">
    {#each popular as movie}
    <MovieCard movies={movie} />
    {/each}
</div>

<style>
    h1
    {
        padding:0 1 rem;
    }

    .popularMovies
    {
        display:grid;
        grid-template-columns: repeat(autoFit, minmax(250px, 1fr));
        grid-column-gap:1rem;
        grid-row-gap:2rem;
    }
</style>