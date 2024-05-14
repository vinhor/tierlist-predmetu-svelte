<script>
    export let zobrazeno;
    export let cisloPredmetu;
    import predmety from "./../lib/predmety.json"
</script>
{#if zobrazeno === cisloPredmetu}
<h1>{predmety[cisloPredmetu].name}</h1>
<ul>
    {#each predmety[cisloPredmetu].body as bodPredmetu}
        <li>{bodPredmetu}</li>
    {/each}
</ul>
{/if}