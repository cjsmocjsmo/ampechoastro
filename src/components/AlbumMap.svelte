<script>
        export let AlbID;
        import { albumidstore } from "./IDStore.js";
        
</script>

<ul
        class="grid xxsm:grid-cols-2 xsm:grid-cols-2 sm:grid-cols-3 md:grid-cols-3 lg:grid-cols-3 gap-2 flex items-center"
>
        {#each AlbID as d}
                <button on:click={() => albumidstore.set(d.albumid)} class="min-w-fit text-white">{d.album}</button>
        {/each}
</ul>
