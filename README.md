# Testseiten für den Live-Check (Reply42 Hub, Pages)

Zwei öffentliche Testseiten mit **synthetischem Text** für den automatischen Live-Check des Pages-Moduls im Reply42 Hub (Ende-zu-Ende-Test des Abgleichs zwischen freigegebener Fassung und Live-Seite):

- `seite-a.html`: weicht in genau einem Satz von der Fassung ab (erwartet: eine fehlende und eine zusätzliche Stelle).
- `seite-b.html`: entspricht der Fassung (erwartet: keine Abweichung).

Die Dateien sind byte-gleich zu `reply42-hub/src/lib/pages/testseiten/live-testseite-{a,b}.html` (Zeilenende LF). Nicht ändern, ohne die Quelle im Hub mitzuziehen. Kein echtes Produkt, keine Kundendaten.
