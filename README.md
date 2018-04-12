# Bakalaura/ maģistra darba paraugs

## Vispārīgs apraksts
Šis kods ir no K: diska ( smb://irbe/pub/Admin/ITML/LaTeX-sagataves )

Tas ir ļoti vienkāršs piemērs, bet pamata elementu funkcionalitāte (atsauces, numerācija, Satura rādītājs u.t.t.) darbojas.

Nodaļas un apakšnodaļas, protams, ir vieglāk rakstīt atsevišķos failus, un pēc tam ar include likt masterdokumentā.

## Tehniskā puse
Lai šo tex dabūtu uz PDF, nepieciešams xelatex (xetex), kam savukārt vajadzīgs LaTeX.

### Uzstādīšana
#### Linux
#### Windows

### Kompilēšana
#### Linux
Komanda TEX->PDF:

> xelatex -interaction=nonstopmode darbs-sagatave.tex

vai

> xetex -interaction=nonstopmode darbs-sagatave.tex

Korektas atsauces un numerācijas uzrādās tikai pēc 3. reizes

> xelatex darbs-sagatave.tex && bibtex darbs-sagatave && xelatex darbs-sagatave.tex && xelatex darbs-sagatave.tex

## Failu struktūra

    /src - visi tex un bib faili
      .bib - bibliogrāfisko atsauču faili http://www.bibtex.org/Format/
      .tex - visi tex faili, kurus esam atdalījuši no galvenā faila
    /images
      /internet - var novietot no interneta paņemtās bildes
      /generated - var novietot pašu veidotos attēlus
