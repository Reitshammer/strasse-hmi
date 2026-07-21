# RoadVision Live

Mobile Web-App zur lokalen Live-Erkennung von Fahrbahnmarkierungen. Die Aufnahmen werden ausschließlich im Smartphone-Browser verarbeitet und nicht hochgeladen.

## Auf GitHub Pages veröffentlichen

1. Den Inhalt dieses Ordners in ein neues GitHub-Repository hochladen.
2. In GitHub **Settings → Pages → Build and deployment → Source** auf **GitHub Actions** stellen.
3. Unter **Actions** den automatisch gestarteten Ablauf abwarten.
4. Die angezeigte HTTPS-Adresse am Smartphone öffnen und den Kamerazugriff erlauben.

## Sicherer Fahrtest

- Smartphone stabil und vibrationsarm mittig hinter der Windschutzscheibe montieren.
- Querformat verwenden; Motorhaube und Himmel möglichst außerhalb der grünen Erkennungszone lassen.
- Die Bedienung erfolgt nur im Stillstand oder durch einen Beifahrer.
- Vor der Kundenfahrt dieselbe Strecke bei ähnlichem Licht testen und im Reiter **Kalibrierung** anpassen.

## Unterstützte Browser

- Android: aktuelle Version von Chrome oder Edge
- iPhone: aktuelle Version von Safari; über **Teilen → Zum Home-Bildschirm** installierbar

Kamerazugriff funktioniert im Browser nur über HTTPS. GitHub Pages stellt HTTPS automatisch bereit.

## Funktionen

- Live-Erkennung weißer und optional gelber Fahrbahnmarkierungen
- stabilisierte Versatzanzeige mit Status für linke/rechte Markierung
- Kalibrierungs- und Einstellreiter mit Hilfetexten
- integrierter Demo-Modus für Präsentationen
- offline startbar, nachdem die App einmal geladen wurde
- keine Cloud-Verarbeitung und keine externen Bibliotheken zur Laufzeit
