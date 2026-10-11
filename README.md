# EA 4: Parametrisierte Flächen

Einsendeaufgabe 4, Modul Graphical Visualisation Technologies, TH Lübeck, Wintersemester 2026/27.

Eine einseitige Web-App mit rohem WebGL 1. Drei parametrisierte Flächen werden
algorithmisch aus einem Parametergitter in u und v erzeugt, als Linienmodell und
als gefüllte, farbig verlaufende Fläche gezeigt. Zwei Flächen stammen aus dem
Material von J. Meier (Dini-Fläche, Seashell), die dritte (Qualle) ist eine
eigene Parametrisierung. Die Formeln stehen auf der Seite.

## Live-Demo

Öffentlich erreichbar unter:
<https://merganh.github.io/gvt-ea4-parametrisierte-flaechen/>

## Lokal ausführen

Kein Build-Schritt. Die Seite lässt sich über einen lokalen Server öffnen:

```bash
python3 -m http.server 8000
# dann im Browser: http://localhost:8000
```

## Deployment via GitHub Pages

Im Repo liegt ein Workflow unter `.github/workflows/pages.yml`, der die Seite bei
jedem Push auf `main` automatisch nach GitHub Pages deployt. Einmalig im Repo
unter **Settings → Pages → Build and deployment → Source** `GitHub Actions`
wählen.

## Aufbau

- `index.html`: gesamte Anwendung in einer Datei (HTML, CSS, JS inline)

Es werden keine externen Bibliotheken oder Dateien geladen.

## Bedienung

- **B**: zur nächsten Fläche wechseln (Dini-Fläche, Seashell, Qualle)
- **F**: zwischen gefüllter Fläche mit Linien und reinem Linienmodell umschalten

Jede Taste hat einen gleichnamigen Button. Gedrückthalten wiederholt nicht.

## Quelltext-Markierung

Die für die Aufgabe geschriebenen JavaScript-Stellen sind mit
`// START EA4_PARAMETRISIERTE_FLAECHEN` und
`// END EA4_PARAMETRISIERTE_FLAECHEN` markiert.
