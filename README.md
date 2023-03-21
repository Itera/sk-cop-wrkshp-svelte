# Run project

- `npm run dev`
- `yarn dev`

# Poznamocky #
- Vsecko je dokopy, HTML, CSS aj JS v jednom fajle `*.svelte`
- Routovanie je file-system based. Jak si das foldery a v nich `+page.svelte` (akoze index) fajly, taku mas routu
- Podľa ["real world"](https://github.com/sveltejs/realworld) appky od Svelte sa komponenty dávajú priamo do zložky `routes`
- Ak chcem do komponentu vnoriť nejaký iný komponent, urobím to prostredníctvom `<slot></slot>`
- TypeScript sa v rámci IntelliJ nesťažuje na to, na čo by sa sťažovať mal (napr. chýbajúca prop keď volám komponent). Odporúčam mať pustený `npm run check:watch` a pravidelne ho kontrolovať - on tieto veci zachytí.
