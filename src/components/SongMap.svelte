<script>
    export let SonID;
    import { songidstore } from "./IDStore.js";
    
</script>

<ul
    class="grid xxsm:grid-cols-2 xsm:grid-cols-2 sm:grid-cols-3 md:grid-cols-3 lg:grid-cols-3 gap-2 flex items-center"
>
    {#each SonID as d}
            <button on:click={() => songidstore.set(d.songid)} class="min-w-fit text-white">{d.song}</button>
    {/each}
</ul>
