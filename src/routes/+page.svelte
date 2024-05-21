<script>
  import "./../lib/style.css";
  import TableElement from "./TableElement.svelte";
  let zobrazeno;
</script>

<h1>Tierlist předmětů</h1>
<main>
<table>
<tbody>
  <tr>
    <th scope="row">S</th>
    <td><button on:click={() => zobrazeno = 0}>Fy</button></td>
    <td><button on:click={() => zobrazeno = 5}>D</button></td>
  </tr>
  <tr>
    <th scope="row">A</th>
    <td><button on:click={() => zobrazeno = 1}>M</button></td>
    <td><button on:click={() => zobrazeno = 7}>Čjl</button></td>
  </tr>
  <tr>
    <th scope="row">B</th>
    <td><button on:click={() => zobrazeno = 4}>Z</button></td>
    <td><button on:click={() => zobrazeno = 8}>Bi</button></td>

  </tr>
  <tr>
    <th scope="row">C</th>
    <td><button on:click={() => zobrazeno = 3}>Ov</button></td>
    <td><button on:click={() => zobrazeno = 6}>Čjm</button></td>
  </tr>
  <tr>
    <th scope="row">D</th>
    <td><button on:click={() => zobrazeno = 2}>Ch</button></td>
    <td><button on:click={() => zobrazeno = 9}>Aj</button></td>
  </tr>
  </tbody>
</table>
<TableElement {zobrazeno} cisloPredmetu={0} />
<TableElement {zobrazeno} cisloPredmetu={1} />
<TableElement {zobrazeno} cisloPredmetu={2} />
<TableElement {zobrazeno} cisloPredmetu={3} />
<TableElement {zobrazeno} cisloPredmetu={4} />
<TableElement {zobrazeno} cisloPredmetu={5} />
<TableElement {zobrazeno} cisloPredmetu={6} />
<TableElement {zobrazeno} cisloPredmetu={7} />
<TableElement {zobrazeno} cisloPredmetu={8} />
<TableElement {zobrazeno} cisloPredmetu={9} />
</main>