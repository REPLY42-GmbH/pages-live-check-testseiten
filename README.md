# Testseiten für den Live-Check (Reply42 Hub, Pages)

Zwei öffentliche Testseiten mit **synthetischem Text** für den automatischen Live-Check des Pages-Moduls im Reply42 Hub (Ende-zu-Ende-Test des Abgleichs zwischen freigegebener Fassung und Live-Seite):

- `seite-a.html`: weicht in genau einem Satz von der Fassung ab (erwartet: eine fehlende und eine zusätzliche Stelle).
- `seite-b.html`: entspricht der Fassung (erwartet: keine Abweichung).
- `seite-c.html`: Hülle wie B, im `main` unverändert das Lieferobjekt eines synthetischen Abnahme-Inhalts (erwartet: keine Abweichung); keine Quelle im Hub.
- `seite-d.html`: Hülle wie C, im `main` unverändert das Lieferobjekt des synthetischen Abnahme-Inhalts „Infografik L18“ mit Bilddatei `seite-dhtml-r42-6dda208c4dc4.png` (erwartet: keine Abweichung).
- `seite-e.html`: wie D, aber das `img` verweist auf eine ältere Bildversion (`seite-dhtml-r42-dfcad256d257.png`, gleicher Alt-Text; erwartet: `bild_veraltet`). Die Bilddatei ist eine Kopie der Datei aus D, damit die Seite vollständig lädt.
- `seite-f.html`: Hülle wie D, im `main` unverändert das Lieferobjekt des synthetischen Abnahme-Artikels „E2E L19 D1b: 7 Tipps für ein sicheres Bad im Alter“ (Lauf 19, ohne Health) mit seinen Bilddateien; nur das Autorenfoto liegt als lokale Kopie `seite-f-autor.png` vor (erwartet: keine Abweichung). Seit Lauf 20 (Testseite H) trägt sie die überarbeitete Fassung aus dem Refresh desselben Artikels, mit allen Bildern unter ihren gelieferten Dateinamen (erwartet: keine Abweichung).
- `seite-g.html`: Hülle wie D, im `main` unverändert das Lieferobjekt des synthetischen Abnahme-Artikels „E2E L19 D2: 5 Tipps für mehr Bewegungsfreiheit im Bad“ (Lauf 19, mit Health und Infografik) mit seinen Bilddateien; nur das Autorenfoto liegt als lokale Kopie `seite-g-autor.png` vor (erwartet: keine Abweichung).

- `seite-l23-fr-a.html`: Lauf 23, Fall A (Sprachfassung `fr-FR` ohne Marktkontakt): im `main` unverändert das Lieferobjekt, Hülle mit `lang="fr"` (erwartet: keine Abweichung).
- `seite-l23-fr-b.html`: Lauf 23, Fall B (Sprachfassung `fr-FR` mit Marktkontakt): wie A (erwartet: keine Abweichung).
- `seite-l23-fr-b-deutsch.html`: wie `seite-l23-fr-b.html`, aber mit synthetischem deutschem Text (erwartet: Abweichungen, Rückgabe an die Umsetzung).

Die Dateien sind byte-gleich zu `reply42-hub/src/lib/pages/testseiten/live-testseite-{a,b}.html` (Zeilenende LF). Nicht ändern, ohne die Quelle im Hub mitzuziehen. Kein echtes Produkt, keine Kundendaten.
