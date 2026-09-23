# Kino – adgangskontroll

Dette er en enkel nettside som sjekker om en person kan få adgang til kinoen. Brukeren skriver inn alderen sin og huker av dersom en foresatt er med. Når brukeren trykker på **Sjekk adgang**, viser nettsiden om personen kommer inn alene, kommer inn med foresatt eller ikke kommer inn.

## Funksjonalitet

- Brukeren skriver inn alder i et tallfelt.
- Brukeren kan huke av for at en foresatt er med.
- Personer som er 15 år eller eldre får adgang uten foresatt.
- Personer fra 12 til 14 år får adgang dersom de har med foresatt.
- Personer under 15 år uten foresatt får ikke adgang.
- Personer under 12 år får ikke adgang selv om de har med foresatt.
- Resultatet vises både på nettsiden og i konsollen.

## JavaScript jeg har brukt

- en funksjon som kjøres ved knappetrykk
- `document.querySelector()` for å finne HTML-elementer
- `.value` for å lese alder
- `.checked` for å kontrollere checkboxen
- `if`, `else if` og `else` for å ta valg
- sammenligningsoperatorer og den logiske operatoren `&&`
- endring av innhold på nettsiden
- `console.log()` for å vise resultatet i konsollen

## Designvalg

Jeg valgte svart bakgrunn og hvit tekst fordi jeg ofte arbeider i et mørkt rom. En hvit bakgrunn blir veldig lys og ubehagelig for øynene, mens det mørke designet blender mindre og gjør nettsiden mer behagelig å arbeide med. Den sterke kontrasten mellom svart og hvitt gjør også teksten lett å lese.

## Slik brukes nettsiden

1. Skriv inn alderen din.
2. Huk av **Jeg har med foresatt** dersom en foresatt er med.
3. Trykk på **Sjekk adgang**.
4. Les resultatet på nettsiden eller i nettleserkonsollen.

## Teknologi

- HTML
- CSS
- JavaScript

## Bruk av AI

Jeg laget HTML-, CSS- og JavaScript-koden selv. AI hjalp meg bare med ideen om å bruke en `<label>` til checkboxen og med å skrive denne Markdown-filen. AI skrev ikke løsningen eller adgangslogikken for meg.
