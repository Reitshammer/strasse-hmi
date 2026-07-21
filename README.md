# RoadVision Live

Mobile Web-App zur lokalen Live-Erkennung von Fahrbahnmarkierungen. Die Aufnahmen werden ausschließlich im Smartphone-Browser verarbeitet und nicht hochgeladen.

## Auf GitHub Pages veröffentlichen

1. Den Inhalt dieses Ordners in das GitHub-Repository hochladen.
2. In GitHub **Settings → Pages → Build and deployment → Source** auf **Deploy from a branch** stellen.
3. Als Branch **main** und als Ordner **/(root)** auswählen und speichern.
4. Den erfolgreichen Pages-Einsatz abwarten und anschließend die HTTPS-Adresse am Smartphone öffnen.

Ein versteckter `.github`-Ordner wird für diese Veröffentlichung nicht benötigt.

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
- gezielte Einzelmarkierungs-Erkennung: **Links**, **Mitte** oder **Rechts** im Kamerabild
- es wird immer nur die ausgewählte Linie gesucht, verfolgt und hervorgehoben
- stabilisierte Abweichungsanzeige zur gewählten Sollposition
- sichtbarer logischer Schaltausgang mit getrennten EIN-/AUS-Schaltpunkten
- einstellbare Hysterese gegen schnelles Flattern des Ausgangs
- vollständige Statusanzeige auch im Smartphone-Querformat
- Kalibrierungs- und Einstellreiter mit Hilfetexten
- integrierter Demo-Modus für Präsentationen
- offline startbar, nachdem die App einmal geladen wurde
- keine Cloud-Verarbeitung und keine externen Bibliotheken zur Laufzeit

## Ziellinie auswählen

Unter **Einstellungen → Ziellinie auswählen** die Position **Links**, **Mitte** oder **Rechts** wählen und speichern. Diese Auswahl steht in Version 1.2 besonders hervorgehoben ganz oben. Die Angabe bezieht sich auf die Position im Kamerabild, nicht auf die rechtliche Art der Markierung. In der Live-Anzeige steht die aktive Auswahl zusätzlich oben als `ZIEL`.

## Schaltausgang

Die Erkennungssicherheit steuert einen logischen Ausgang. Standardmäßig schaltet er bei **50 % EIN** und erst unter **25 % AUS**. Beide Schaltpunkte sind am Sicherheitsbalken markiert und unter **Einstellungen** anpassbar. Zwischen den beiden Punkten behält der Ausgang seinen letzten Zustand. Dadurch flattert er bei schwankender Erkennung nicht.

Die Web-App zeigt den logischen Ausgang an. Ein physischer elektrischer Ausgang benötigt weiterhin eine Anbindung an die spätere Steuerung oder Hardware.

## Aktualisierung von einer älteren Version

Version 1.3 lädt die Startseite bevorzugt aus dem Netz und ersetzt ältere Offline-Dateien automatisch. Nach dem Hochladen GitHub Pages einmal vollständig neu laden. Im Kopfbereich und unten in den Einstellungen muss **V1.3** stehen. Falls eine am Home-Bildschirm installierte ältere Version erscheint, diese Verknüpfung einmal entfernen, die GitHub-Pages-Seite neu öffnen und anschließend wieder zum Home-Bildschirm hinzufügen.
