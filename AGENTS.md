# AGENTS.md

## Project

Dit is de WordPress-website van Vereniging De Oude Beek.

Staging:
- experiment.deoudebeek.nl

Technische basis:
- WordPress
- Gutenberg en Full Site Editing
- Parent theme: Twenty Twenty-Five
- Child theme: `de-oude-beek-foundation`
- Projectfunctionaliteit: `de-oude-beek-core`, indien aanwezig

## Bronnen

Lees vóór iedere implementatietaak:

1. `docs/Technische_implementatiespecificatie_CODEX_De_Oude_Beek_v1.0.docx`
2. `docs/Definitief_tekst_en_blokmodel_De_Oude_Beek_v0.1.docx`

De technische specificatie bepaalt hoe de website wordt gebouwd.
Het tekst- en blokmodel bepaalt de inhoud en paginastructuur.

## Werkprincipes

- Standaard WordPress-functionaliteit waar mogelijk.
- Maatwerk alleen waar nodig.
- Gebruik Gutenberg, Full Site Editing, `theme.json`, templates en patterns.
- Wijzig nooit bestanden van WordPress-core, het parent theme of externe plug-ins.
- Maak geen externe pagebuilder-afhankelijkheid.
- Voeg geen plug-in toe zonder expliciete opdracht.
- Verzin geen inhoud, bedragen, datums, documentstatussen of persoonsgegevens.
- Publiceer conceptbeleid niet als geldende regeling.
- Houd de website mobiel, toegankelijk en beheerbaar zonder programmeerkennis.

## Toegestane codegebieden

Werk alleen in:

- `wp-content/themes/de-oude-beek-foundation/`
- `wp-content/plugins/de-oude-beek-core/`

Wijzig documentatie alleen wanneer de opdracht dit uitdrukkelijk vraagt.

## Niet opnemen

Voeg nooit toe:

- `wp-config.php`
- wachtwoorden of API-sleutels
- database-exporten
- uploads
- back-ups
- logbestanden
- productiegegevens

## Werkwijze

Voor iedere taak:

1. inspecteer eerst de relevante bestaande bestanden;
2. meld conflicten of ontbrekende informatie;
3. maak de kleinst mogelijke samenhangende wijziging;
4. wijzig geen aangrenzende functionaliteit zonder noodzaak;
5. voer beschikbare controles uit;
6. rapporteer gewijzigde bestanden, tests en resterende risico’s.

## Veiligheid

- Werk niet rechtstreeks op productie.
- Voer geen deployment uit zonder expliciete opdracht.
- Verwijder geen bestaande code of inhoud zonder toelichting.
- Bewaar achterwaartse compatibiliteit waar redelijk.
- Gebruik WordPress escaping, sanitization, nonces en capabilities waar van toepassing.

## Toegankelijkheid

Streef naar WCAG 2.2 AA:

- semantische HTML;
- één H1 per pagina;
- toetsenbordbediening;
- zichtbare focus;
- voldoende contrast;
- correcte labels;
- ondersteuning voor `prefers-reduced-motion`.

## Eerste fase

De eerste Codex-opdracht is uitsluitend een inventarisatie.
Wijzig daarbij geen bestanden.
