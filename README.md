<div align="center">

<h1>⚡ Shxrk Launcher</h1>

<p>Ein moderner, kostenloser Launcher für Minecraft: Java Edition</p>

[![Download](https://img.shields.io/badge/Download-Latest-white?style=for-the-badge)](https://github.com/xXSquirtz/ZeroxLauncher/releases/latest)
![Windows](https://img.shields.io/badge/Windows%2010%20%7C%2011-supported-0078D4?style=for-the-badge&logo=windows&logoColor=white)
![macOS](https://img.shields.io/badge/macOS-supported-555555?style=for-the-badge&logo=apple&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-supported-FCC624?style=for-the-badge&logo=linux&logoColor=black)

</div>

---

## 📥 Download

| Plattform | Datei |
|---|---|
| Windows 10 / 11 x64 | `Shxrk-Launcher-Setup-x.y.z.exe` |
| macOS (Intel / Apple Silicon) | `Shxrk-Launcher-x.y.z-x64.dmg` oder `Shxrk-Launcher-x.y.z-arm64.dmg` |
| Linux x64 | `Shxrk-Launcher-x.y.z-x64.AppImage` oder `Shxrk-Launcher-x.y.z-x64.deb` |
| Linux ARM64 / Chromebook ARM | `Shxrk-Launcher-x.y.z-arm64.AppImage` oder `Shxrk-Launcher-x.y.z-arm64.deb` |

> Der Installer erstellt automatisch eine Desktop-Verknüpfung und fügt Shxrk Launcher zu den Windows Apps hinzu.
> Alle Plattformpakete werden bei getaggten GitHub-Releases automatisch gebaut. Lokal: `npm run build:win`, `npm run build:mac` oder `npm run build:linux`; macOS-Builds benötigen macOS.
> macOS-Pakete sind derzeit nicht mit einem Apple-Developer-Zertifikat signiert. Beim ersten Öffnen kann Gatekeeper eine Warnung anzeigen; dann im Finder per Rechtsklick **Öffnen** wählen.

---

## ✨ Features

- 🔑 **Microsoft-Login** – Offizieller OAuth-Login über Microsoft und Xbox Live
- 🚀 **Minecraft Java starten** – Direkt aus dem Launcher, mit automatischer Java-Erkennung
- 🧩 **Instanzen** – Eigene Instanzen mit separatem Spielverzeichnis erstellen und verwalten
- 📦 **Modpacks** – Modrinth Modpacks durchsuchen & mit einem Klick installieren
- 🎛️ **Modpack-Instanzen** – Beim Installieren Instanznamen und Minecraft-Version auswählen; es wird die passende Modpack-Version verwendet
- 🔍 **Mods** – Mods direkt über Modrinth suchen und in Instanzen installieren, aktivieren oder deaktivieren
- ✅ **Kompatible Mods** – Suche und Download berücksichtigen Minecraft-Version und Mod-Loader
- 🦈 **Shxrk Client** – Durchsichtiges Right-Shift-Overview mit Shark-Logo, scrollbarem Feature-Karussell, Keybind-Einstellungen und anpassbaren HUD-Positionen; Linksklick schaltet ein Feature um, Rechtsklick öffnet dessen Einstellungen
- 🎮 **Discord Rich Presence** – Zeigt Minecraft als über den Shxrk Launcher gestartet an, solange Java oder Bedrock läuft
- 🎨 **Skins** – Eigene Minecraft-Skins verwalten und live in 3D vorschauen
- 📋 **Logs** – Alle Minecraft-Logs direkt im Launcher einsehen

### Shxrk Client: unterstützte Kombinationen

| Minecraft | Loader |
|---|---|
| 1.20.1 | Fabric, Quilt, Forge |
| 1.21.1 | Fabric |
| 1.21.11 | Fabric |

Nicht aufgeführte Kombinationen werden vor dem Spielstart mit einer verständlichen Meldung abgewiesen, bis ein passendes Mod-Artefakt verfügbar ist. Dazu gehören derzeit Minecraft 1.8.9, 26.2/26.3 (keine nutzbaren Fabric-Mappings) sowie Forge/Quilt für 1.21.x. Der Installer-Build erzeugt die Minecraft-spezifischen Fabric-JARs und lädt benötigte Loader-Brücken nur von Modrinth; jede heruntergeladene Datei wird vor dem Verpacken per SHA-512 geprüft.

Keybinds und Feature-Einstellungen werden lokal gespeichert. `npm run dev`, `npm start` und `npm run build` bauen die Mod-Artefakte automatisch. Dafür werden der mitgelieferte Gradle Wrapper, ein JDK 21 oder neuer und Internetzugriff auf Fabric/Modrinth benötigt.

---

## 🔒 Sicherheit & Datenschutz

- Der Login nutzt ausschließlich die offiziellen Microsoft / Xbox / Mojang-APIs
- Es werden keine Account-Daten an Dritte übertragen
- Tokens werden ausschließlich lokal auf deinem Gerät gespeichert
- Alle Spiel-Downloads kommen direkt von Mojang und Modrinth

---

## 🖥️ Systemvoraussetzungen

- Windows 10 / 11, macOS oder Linux (64-bit; Linux x64 und ARM64)
- Minecraft: Java Edition (gekauftes Microsoft-Konto)
- Internetverbindung
- Chromebook: Linux-Entwicklungsumgebung (Crostini) aktiviert; ChromeOS selbst führt keine Electron-Desktop-Apps nativ aus
- Chromebook: Paket passend zur Linux-Architektur (x64 oder ARM64) verwenden; für AppImage muss FUSE verfügbar sein, alternativ das `.deb` installieren

Auf Linux-Systemen mit Schlüsselbund (Secret Service) wird der Microsoft-Login verschlüsselt gespeichert. Falls kein Schlüsselbund verfügbar ist, bleibt der Token-Cache aus Sicherheitsgründen nur bis zum Beenden des Launchers im Arbeitsspeicher.

---

## 🇬🇧 About (English)

Shxrk Launcher is a free, modern launcher for Minecraft: Java Edition on Windows, macOS and Linux. On Chromebooks it runs inside the Linux development environment (Crostini); choose the Linux package matching the Chromebook's CPU architecture. It supports vanilla gameplay, custom instances, modpack installation via Modrinth, and mod management. Players sign in with the official Microsoft OAuth 2.0 Device Code Flow. No account data is transmitted to third-party servers.

---

<div align="center">
  <sub>© 2026 _xno · Nicht mit Mojang oder Microsoft verbunden.</sub>
</div>
