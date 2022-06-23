<script>
    export /**
* @type {any}
*/
     let movies;
</script>


<div class="movieCard">
    <img src="{ 'https://image.tmdb.org/t/p/w500' + movies.poster_path}" alt="{movies.title}" />
</div>

<div class="description">
    <h2>{movies.title}</h2>
    <p>
        {movies.release_date}
    </p>
</div>