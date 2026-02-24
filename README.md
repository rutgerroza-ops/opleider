# Handboek secundaire arbeidsvoorwaarden (mobiel, geen website)

Voor een **mobiele versie van een handboek die géén website is**, is dit in de praktijk een sterk format:

## Aanbevolen format

1. **Bronbestand in Markdown (`handboek.md`)**
   - Makkelijk te onderhouden in Git.
   - Duidelijke koppenstructuur en versiebeheer.

2. **Distributie als EPUB (primair)**
   - Geoptimaliseerd voor smartphone-leesapps (Apple Books, Google Play Books, Kobo, etc.).
   - Reflowable tekst: past zich automatisch aan schermgrootte en letterinstellingen aan.

3. **Optioneel PDF (secundair)**
   - Handig voor print of formele archivering.
   - Minder flexibel op kleine schermen dan EPUB.

## Waarom dit beter is dan een website voor jouw vraag

- Werkt offline in leesapps.
- Geen hosting, domein of browser-UI nodig.
- Medewerkers kunnen bladwijzers, highlights en notities gebruiken.

## Structuur van het handboek

Gebruik het sjabloon in [`handboek.md`](./handboek.md) met:
- korte hoofdstukken;
- duidelijke tussenkoppen;
- bullets i.p.v. lange alinea's;
- per regeling: *Wat is het?*, *Voor wie?*, *Voorwaarden*, *Aanvragen*.

## Exporteren naar EPUB/PDF (met Pandoc)

```bash
# EPUB
pandoc handboek.md -o handboek.epub

# PDF
pandoc handboek.md -o handboek.pdf
```

## Publicatie-advies op smartphone

- Deel `handboek.epub` via intranet, Teams of e-mail.
- Adviseer medewerkers om het bestand te openen in een e-reader app.
- Gebruik versienummers in bestandsnaam, bijvoorbeeld: `handboek-arbeidsvoorwaarden-v1.2.epub`.
