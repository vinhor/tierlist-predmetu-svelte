<script>
  import "./../lib/style.css";
  import TableElement from "./TableElement.svelte";
  const cislaPredmetu = { fyzika: 0, matematika: 1, chemie: 2, obcanka: 3 }
  let zobrazeno;
</script>

<h1>Tierlist předmětů</h1>
<main>
<table>
<tbody>
  <tr>
    <th scope="row">S</th>
    <td><button on:click={() => zobrazeno = cislaPredmetu.fyzika}>Fy</button></td>
  </tr>
  <tr>
    <th scope="row">A</th>
    <td><button on:click={() => zobrazeno = cislaPredmetu.matematika}>M</button></td>
  </tr>
  <tr>
    <th scope="row">B</th>
    <td><button on:click={() => zobrazeno = cislaPredmetu.chemie}>Ch</button></td>
  </tr>
  <tr>
    <th scope="row">C</th>
  </tr>
  <tr>
    <th scope="row">D</th>
    <td><button on:click={() => zobrazeno = cislaPredmetu.obcanka}>Ov</button></td>
  </tr>
  </tbody>
</table>
<TableElement {zobrazeno} cisloPredmetu={cislaPredmetu.fyzika} />
<TableElement {zobrazeno} cisloPredmetu={cislaPredmetu.matematika} />
<TableElement {zobrazeno} cisloPredmetu={cislaPredmetu.chemie} />
<TableElement {zobrazeno} cisloPredmetu={cislaPredmetu.obcanka} />
</main>