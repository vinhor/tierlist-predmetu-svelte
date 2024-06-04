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
        <td
          ><button
            on:click={() => (zobrazeno = 1)}
            class={zobrazeno === 1 ? "zobrazene" : ""}>M</button
          ></td
        >
        <td
          ><button
            on:click={() => (zobrazeno = 5)}
            class={zobrazeno === 5 ? "zobrazene" : ""}>D</button
          ></td
        >
        <td
          ><button
            on:click={() => (zobrazeno = 10)}
            class={zobrazeno === 10 ? "zobrazene" : ""}>Iv</button
          ></td
        >
      </tr>
      <tr>
        <th scope="row">A</th>
        <td
          ><button
            on:click={() => (zobrazeno = 0)}
            class={zobrazeno === 0 ? "zobrazene" : ""}>Fy</button
          ></td
        >
        <td
          ><button
            on:click={() => (zobrazeno = 7)}
            class={zobrazeno === 7 ? "zobrazene" : ""}>Čjl</button
          ></td
        >
        <td
          ><button
            on:click={() => (zobrazeno = 13)}
            class={zobrazeno === 13 ? "zobrazene" : ""}>Nj</button
          ></td
        >
      </tr>
      <tr>
        <th scope="row">B</th>
        <td
          ><button
            on:click={() => (zobrazeno = 4)}
            class={zobrazeno === 4 ? "zobrazene" : ""}>Z</button
          ></td
        >
        <td
          ><button
            on:click={() => (zobrazeno = 8)}
            class={zobrazeno === 8 ? "zobrazene" : ""}>Bi</button
          ></td
        >
        <td
          ><button
            on:click={() => (zobrazeno = 14)}
            class={zobrazeno === 14 ? "zobrazene" : ""}>Tv</button
          ></td
        >
      </tr>
      <tr>
        <th scope="row">C</th>
        <td
          ><button
            on:click={() => (zobrazeno = 3)}
            class={zobrazeno === 3 ? "zobrazene" : ""}>Vo</button
          ></td
        >
        <td
          ><button
            on:click={() => (zobrazeno = 6)}
            class={zobrazeno === 6 ? "zobrazene" : ""}>Čjm</button
          ></td
        >
        <td
          ><button
            on:click={() => (zobrazeno = 12)}
            class={zobrazeno === 12 ? "zobrazene" : ""}>Vv</button
          ></td
        >
      </tr>
      <tr>
        <th scope="row">D</th>
        <td
          ><button
            on:click={() => (zobrazeno = 2)}
            class={zobrazeno === 2 ? "zobrazene" : ""}>Ch</button
          ></td
        >
        <td
          ><button
            on:click={() => (zobrazeno = 9)}
            class={zobrazeno === 9 ? "zobrazene" : ""}>Aj</button
          ></td
        >
        <td
          ><button
            on:click={() => (zobrazeno = 11)}
            class={zobrazeno === 11 ? "zobrazene" : ""}>Hv</button
          ></td
        >
      </tr>
    </tbody>
  </table>
  <p>
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
    <TableElement {zobrazeno} cisloPredmetu={10} />
    <TableElement {zobrazeno} cisloPredmetu={11} />
    <TableElement {zobrazeno} cisloPredmetu={12} />
    <TableElement {zobrazeno} cisloPredmetu={13} />
    <TableElement {zobrazeno} cisloPredmetu={14} />
  </p>
</main>
<h2>Disclaimer</h2>
<p>Tato stránka je čistě pro pobavení. Trvzení jsou nadsazená.</p>
<p>
  Kódováno pomocí&nbsp;<a href="https://svelte.dev/">Svelte</a>
</p>
