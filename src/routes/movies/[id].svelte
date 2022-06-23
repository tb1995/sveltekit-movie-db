<script context="module">
    
    // @ts-ignore
    export async function load( {fetch, params} )
    {
      console.log(params.id);
      const res = await fetch('https://api.themoviedb.org/3/movie/${params.id}}?api_key=00f18f62f1339acd38f45ceabf0531b5&language=en-US');
      const data = await res.json();
      //console.log(data);
      if (res.ok)
      {
          return {
              props: { data }
          };
      }
    }
</script>