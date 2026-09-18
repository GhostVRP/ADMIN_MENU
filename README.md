# 🛠️ GhostV ADMIN MENU

Version 1.0.0

Ein performantes, modernes und vollständig framework-unabhängiges (**Standalone**) Admin-Menü für FiveM-Server. Entwickelt von **GhostV - HugoHD** für maximale Effizienz, hohe Anpassungsfähigkeit und eine intuitive Benutzeroberfläche.

## ✨ Features

* **⚡ Framework Independent (Standalone):** Funktioniert ohne ESX, QBCore oder VRP. Nur reine FiveM Native-Power.

* **🛡️ Rechte-System:** Integrierte Ace-Permissions zur exakten Gruppen- und Rechtevergabe.

* **👤 Spieler-Management:**

  * Kicken, Bannen, Warnen, Teleportieren (Zu Spieler / Spieler zu mir).

  * Wiederbeleben (Revive), Heilen, Rüstung geben.

  * Inventar/Geld-Verwaltung (optional konfigurierbar).

* **🚗 Fahrzeug-Optionen:**

  * Fahrzeuge spawnen, reparieren, tunen, löschen.

  * Unzerstörbarkeit (Godmode) & Max-Performance.

* **🌐 Server-Tools:**

  * Wetter & Uhrzeit in Echtzeit ändern.

  * Server-Ankündigungen (Announcements) senden.

* **🎨 Modernes UI:** Clean, responsiv und ressourcenschonend (niedriger MS-Resmon-Wert).

## 📥 Installation

1. **Download:** Lade die neueste Version von der [](#) herunter oder klone das Repository.

2. **Ordner platzieren:** Entpacke den Ordner in deinen `resources`-Ordner deines FiveM-Servers (z. B. `resources/[ghostv]/ghostv_admin`).

3. **Server.cfg konfigurieren:** Füge die Ressource zu deiner `server.cfg` hinzu:

   ```
   ensure ghostv_admin
   
   ```

4. **Permissions einrichten:** Gib deiner Admin-Gruppe die entsprechenden Rechte in der `server.cfg`:

   ```
   add_ace group.admin "ghostv.admin.menu" allow
   add_principal identifier.fivem:123456 group.admin
   
   ```

## ⚙️ Konfiguration

Alle wichtigen Einstellungen können in der `config.lua` angepasst werden:

```
Config = {}

-- Standard-Taste zum Öffnen des Menüs
Config.OpenKey = 'F10' 

-- Spracheinstellungen (de / en)
Config.Language = 'de'

-- Discord Webhook für Admin-Logs
Config.DiscordWebhook = "DEINE_DISCORD_LINK"

```

## 🔒 Ace Permissions

Du kannst verschiedene Features mit spezifischen Ace-Permissions absichern:

| Permission | Beschreibung | 
 | ----- | ----- | 
| `ghostv.admin.menu` | Erlaubt das Öffnen des Admin-Menüs | 
| `ghostv.admin.players` | Zugriff auf Spieler-Aktionen (Kick/Ban/TP) | 
| `ghostv.admin.vehicles` | Zugriff auf Fahrzeug-Spawning und Modifikationen | 
| `ghostv.admin.server` | Zugriff auf Server-Einstellungen (Wetter/Zeit) | 

## 👑 Credits & Author

* **Developer:** GhostV - HugoHD

* **Team:** GhostV

## 📝 Lizenz

Dieses Projekt ist unter der **MIT-Lizenz** lizenziert. Weitere Details findest du in der `LICENSE`-Datei.
