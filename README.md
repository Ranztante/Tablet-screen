# Smart Display Dashboard (Samsung Tablet)

Ein minimalistisches, dauerhaftes Smart-Display-Dashboard für ein Android-Tablet, gehostet über GitHub Pages.

## 📱 Übersicht & Features
- **Design:** Android Material Dark Style (`#1e1e1e` / `#000`), optimiert für Tablet-Displays.
- **Obere Hälfte:** Wetter-Widget (`weatherwidget.io`) im Vollbild-Design angepasst an das Android-Dark-Theme (Standort: Leuna).
- **Untere Hälfte:** Google Kalender im sauberen Agenda-Modus.

---

## 🛠️ Technische Einrichtung & Komponenten

### 1. Web-Interface (`index.html`)
Das Dashboard besteht aus einer einzigen `index.html`-Datei im Repository, die via **GitHub Pages** bereitgestellt wird:
- **URL:** `https://ranztante.github.io/Tablet-screen/`
- **Struktur:** Flexbox-Layout mit `100vh`, aufgeteilt in Wetter-Container und Kalender-Iframe.

### 2. Browser-Konfiguration (Via Browser)
Es wird der **Via Browser** verwendet, da dieser im Gegensatz zu strengeren Datenschutz-Browsern (wie Firefox oder Aloha) die für den Google-Kalender notwendigen Cookies reibungslos akzeptiert.
- **Startseite:** Die GitHub-Pages-URL ist als feste Startseite im Via Browser hinterlegt.

### 3. Automatischer Start beim Hochfahren (Autostart)
Um sicherzustellen, dass das Dashboard nach einem Neustart des Tablets sofort wieder da ist:
- **App:** *AutoStart App Manager*
- **Funktion:** Startet den Via Browser automatisch beim Systemstart (*Gerät neugestartet*).

### 4. Dauerhaft aktiver Bildschirm ("No Sleep")
Damit das Display im Betrieb nicht ausgeht:
- **Android-Entwickleroptionen:** Die Option **"Wach bleiben während des Ladens"** ist aktiviert (das Tablet hängt dauerhaft am Ladekabel).
