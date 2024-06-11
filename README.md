# Tierlist předmětů (Svelte)

1. Soubory webové stránky jsou v `src/routes/` na větvi _main_. Zde je komponenta TableElement a stránka samotná.
2. V `src/lib` na větvi _main_ je CSS a JSON s informacemi o předmětech.
3. Vše ostatní je automaticky vygenerované při založení projektu.
4. Na větvi _pages_ jsou data, vygenerovaná pomocí příkazu `npm run build`. Ten převede soubory .svelte na .js a .html
