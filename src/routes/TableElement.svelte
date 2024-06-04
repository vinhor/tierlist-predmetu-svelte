<script>
    export let zobrazeno;
    export let cisloPredmetu;
    import predmety from "./../../static/predmety.json"
</script>
{#if zobrazeno === cisloPredmetu}
<div>
<h1>{predmety[cisloPredmetu].name}</h1>
<ul>
    {#each predmety[cisloPredmetu].body as bodPredmetu}
        <li>{bodPredmetu}</li>
    {/each}
</ul></div>
{/if}
<style>
    div {
        margin: 2rem;
        border: 2px solid #a2adbd;
        padding: 1rem;
    }
    h1 {
        border: none;
    }
</style>