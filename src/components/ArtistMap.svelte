<script>
        // import { artistidstore } from "./IDStore.js";
        export let ArtID;

        // function setArtID(aid) {
        //         console.log("This is from artistmap");
        //         console.log(aid)
        //         localStorage.setItem("artistid", aid)
        // }
</script>

<ul
        class="grid xxsm:grid-cols-2 xsm:grid-cols-2 sm:grid-cols-3 md:grid-cols-3 lg:grid-cols-3 gap-2 flex items-center"
>
        {#each ArtID as d}
                <button
                        id={d.artistid}
                        on:click={() => localStorage.setItem("artistid", d.artistid)}
                        class="min-w-fit text-white"
                        >{d.artist}</button
                >
        {/each}

        
</ul>
