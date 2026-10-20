# Snake

Ein klassisches Snake-Spiel im Browser – gebaut mit HTML5 Canvas.

## [▶ Spiel starten](https://KorayAgl.github.io/snake-game)

## Steuerung
<<<<<<< HEAD
- **Pfeiltasten / WASD / Wischen** – Schlange lenken
- **Enter / R** – Start / Neustart
- **M** – Ton an/aus

## Online-Bestenliste einrichten (Firebase)

Ohne Einrichtung werden Highscores nur im eigenen Browser gespeichert.
Für eine gemeinsame Live-Bestenliste (kostenlos):

1. Auf [console.firebase.google.com](https://console.firebase.google.com) ein neues Projekt anlegen (Google Analytics kann aus bleiben).
2. Links **Build → Firestore Database → Datenbank erstellen** → **Produktionsmodus**, Standort z. B. `eur3 (europe-west)`.
3. Im Tab **Regeln** den Inhalt von [`firestore.rules`](firestore.rules) einfügen und **Veröffentlichen**.
4. In der Projektübersicht auf das Web-Symbol **`</>`** klicken, eine App registrieren (Hosting nicht nötig) und das angezeigte `firebaseConfig`-Objekt kopieren.
5. In `index.html` die Zeile `const FIREBASE_CONFIG = null;` durch die kopierte Konfiguration ersetzen:
   ```js
   const FIREBASE_CONFIG = {
     apiKey: "...",
     authDomain: "...",
     projectId: "...",
     appId: "...",
   };
   ```
6. Committen und pushen – fertig. Oben in der Bestenliste steht dann **● Live**.

Hinweis: Der `apiKey` ist kein Geheimnis, er darf öffentlich im Code stehen. Geschützt wird die Datenbank durch die Regeln in `firestore.rules`.
=======
- **Pfeiltasten** – Schlange lenken
>>>>>>> 36346ad068f8cadaf368a785150b5ec49d1647de
