<script>
  import "./../lib/style.css";
  import TableElement from "./TableElement.svelte";
  const cislaPredmetu = { fyzika: 0 }
  let zobrazeno;
</script>

<h1>Tierlist učitelů</h1>
<main>
<table>
<tbody>
  <tr>
    <th scope="row">S</th>
    <td><button on:click={() => zobrazeno = cislaPredmetu.fyzika}>Fy</button></td>
  </tr>
  <tr>
    <th scope="row">A</th>
  </tr>
  <tr>
    <th scope="row">B</th>
  </tr>
  <tr>
    <th scope="row">C</th>
  </tr>
  <tr>
    <th scope="row">D</th>
  </tr>
  </tbody>
</table>
<TableElement {zobrazeno} cisloPredmetu={cislaPredmetu.fyzika} />
</main>