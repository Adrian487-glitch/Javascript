# Grunnleggende JavaScript

Dette prosjektet inneholder 15 grunnleggende JavaScript-oppgaver samlet på én HTML-side. Oppgavene bygger gradvis videre på hverandre og viser hvordan JavaScript kan brukes sammen med HTML og CSS.

## Dette har jeg jobbet med

- `const` og `let`
- datatyper og `typeof`
- utskrift med `console.log()`
- DOM og `document.querySelector()`
- hendelser med `onclick`
- funksjoner, parametre, argumenter og `return`
- lesing av input med `.value`
- endring av innhold med `.textContent`
- endring av CSS med `.style`
- objekter, egenskaper, metoder og `this`
- en klikk-teller
- et elevkort laget fra brukerens input

## Oppgavene

1. Opprette og skrive ut en variabel.
2. Endre en variabel med `let`.
3. Undersøke forskjellige datatyper.
4. Finne et HTML-element med DOM.
5. Endre tekst på nettsiden.
6. Kjøre en funksjon ved et knappetrykk.
7. La en knapp endre nettsiden.
8. Lese et navn fra et input-felt.
9. Lage en funksjon med parameter og returverdi.
10. Bruke flere parametre og input-felt.
11. Endre CSS med JavaScript.
12. Telle antall knappetrykk.
13. Lage et objekt som representerer en elev.
14. Legge til en metode i elevobjektet.
15. Lage et elevkort fra brukerens navn, alder og klasse.

## Kjør prosjektet

Prosjektet krever ingen installasjon.

1. Åpne `index.html` i en nettleser, eller bruk Live Preview i VS Code.
2. Test knappene og input-feltene på siden.
3. Åpne nettleserens utviklerverktøy for å se utskrifter i konsollen. Dette kan vanligvis gjøres med `F12`.

## Prosjektfiler

```text
javascript/
├── index.html
└── README.md
```

## Ekstraarbeid

I tillegg til kravene i oppgavene har jeg:

- laget et eget mørkt design fordi siden brukes i et mørkt rom, slik at skjermen blender mindre og er mer behagelig å arbeide med
- valgt egne farger og monospace-skrift for overskriftene
- lagt inn hjelpetekster som viser hvor resultatene kan finnes
- brukt `type="number"` på input-felt for alder
- brukt unike ID-er for å holde input-feltene i de forskjellige oppgavene fra hverandre
- testet siden fortløpende med Live Preview og nettleserkonsollen
- feilsøkt blant annet variabelnavn, store og små bokstaver, klammer og funksjonskall
- dokumentert prosjektet med denne README-filen

## Sluttoppgaven

I den siste oppgaven skriver brukeren inn navn, alder og klasse. JavaScript henter verdiene, oppretter et elevobjekt, bruker objektets `presenter()`-metode, viser resultatet på nettsiden, endrer utseendet på elevkortet og skriver objektet til konsollen.
