Quellen zu einem Vortrag zu DNN-Absicherung
===========================================
Dies sind die Quellen zu einem Vortrag zur Absicherung von Deep Neural
Networks (DNNs), der am 20.12.2018 im Rahmen des Lehrstuhlseminars der
Gruppe kognitive Systeme an der Uni Bamberg gehalten wurde.

Die Präsentation wurde mithilfe des LaTeX
[beamer](http://tug.ctan.org/macros/latex/contrib/beamer/doc/beameruserguide.pdf)
Pakets erstellt, wodurch Inhalt mit Notizen und Folienanweisung in
einer Datei zu finden sind.

Quellen für verwendete Bilder sind im Inhalt verlinkt, sofern nicht
selbst erstellt.


## Kompilieren
Getestet mit einer TeXLive 2018 Distribution.

### Notizen
Für die Notizenversion im Terminal eingeben:
```bash
lualatex DNN-Absicherung_Notizen.tex
biber DNN-Absicherung
lualatex DNN-Absicherung_Notizen.tex
```

### Handout/Folien
Relevante Einstellungsmöglichkeiten in den Dokumentenklassenoptionen
in der Datei `DNN-Absicherung_Folien.tex`:
- `aspectratio`: Seitenverhältnis
  - auskommentiert: 4:3
  - `169`: 16:9
- `handout`: Ob eine Handoutversion erzeugt wird
  - auskommentiert bzw. false: Folienversion (Overlays werden eingebaut)
  - einkommentiert bzw. true: Handoutversion (nur eine Seite pro Folie)

Für eine Folien-/Handoutversion im Terminal eingeben:
```bash
lualatex DNN-Absicherung_Folien.tex
biber DNN-Absicherung
lualatex DNN-Absicherung_Folien.tex
```

## Dateien
- `DNN-Absicherung.tex`: Inhalt (sowohl Folien/Handout und Notizen);
  nicht kompilierfähig!
- `DNN-Absicherung_Folien.tex`: Header Datei für Folien/Handout
- `DNN-Absicherung_Notizen.tex`: Header Datei für ausführliche Notizen, d.h. Paper-Format
- `*.bib`: Literatursammlung (erstellt mit Zotero)
- `DNN-Absicherung_Folien_[4zu3|16zu9].pdf`: 4:3 bzw. 16:9 Folien
- `DNN-Absicherung_Handout.pdf`: 4:3 Handout
