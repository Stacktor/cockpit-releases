# cockpit — Downloads

Fertige Installer von **Bewerbungs-Cockpit**: dem Bewerbungsmanager, der deine Daten auf deinem
Gerät lässt. Website: **[cockpit.mesco.cc](https://cockpit.mesco.cc)**

> **Status: geschlossene 0.1 Alpha.** Die App läuft ohne Konto. Mit einem Alpha-Schlüssel sind
> alle Funktionen frei. → [Alpha-Zugang anfragen](https://cockpit.mesco.cc/alpha/)

## Herunterladen

| System | Status | Datei (immer die neueste Version) |
|---|---|---|
| **Windows** 10/11, 64 Bit | ✅ verfügbar | [`cockpit-windows-setup.exe`](https://github.com/Stacktor/cockpit-releases/releases/latest/download/cockpit-windows-setup.exe) · [`cockpit-windows.msi`](https://github.com/Stacktor/cockpit-releases/releases/latest/download/cockpit-windows.msi) |
| **Linux** x86_64 | ✅ verfügbar | [`cockpit-linux-x86_64.AppImage`](https://github.com/Stacktor/cockpit-releases/releases/latest/download/cockpit-linux-x86_64.AppImage) · [`cockpit-linux-amd64.deb`](https://github.com/Stacktor/cockpit-releases/releases/latest/download/cockpit-linux-amd64.deb) |
| **macOS** | 🚧 in Arbeit | vorerst kein Installer |
| **iPhone · iPad** | 🚧 in Arbeit | vorerst nicht verfügbar |

Die Dateinamen bleiben über alle Versionen gleich, Links darauf funktionieren also dauerhaft.
Alle Versionen stehen unter [Releases](https://github.com/Stacktor/cockpit-releases/releases),
was sich geändert hat im [Changelog](https://cockpit.mesco.cc/changelog/).

## Erster Start

- **Windows:** Die Installer sind noch nicht code-signiert. Windows („SmartScreen“) warnt deshalb
  einmal: **Weitere Informationen → Trotzdem ausführen**. Microsoft WebView2 richtet der
  Installer bei Bedarf selbst ein.
- **Linux (AppImage):** `chmod +x cockpit-linux-x86_64.AppImage`, dann starten. Fehlt FUSE:
  `sudo apt install libfuse2`. Gebraucht werden WebKitGTK 4.1 und ein Schlüsselbund
  (GNOME-Schlüsselbund oder KWallet) für Passwörter und API-Schlüssel.
- **Einrichtung:** Der Willkommens-Assistent führt durch Profil, KI und Alpha-Schlüssel.
  Anleitung: [Erste Schritte](https://cockpit.mesco.cc/hilfe/erste-schritte/).

## Updates

cockpit prüft beim Start, ob es eine neue Version gibt, und installiert sie erst auf deinen
Klick. Die Update-Pakete sind signiert, und die App nimmt nur Pakete mit gültiger Signatur an.
Die Update-Information (`latest.json`) liegt im jeweils neuesten Release in diesem Repo.

## Datenschutz in einem Satz

Bewerbungen, Profil, Dokumente und Mails liegen in einer Datenbank auf deinem Rechner,
Schlüssel und Passwörter im Schlüsselbund deines Systems. Es gibt kein Konto und keine Telemetrie.
→ [Datenschutzerklärung](https://cockpit.mesco.cc/datenschutz/)

## Fehler gefunden?

In der App unter **Feedback → Fehler melden**. Bevor etwas gesendet wird, siehst du genau, was
rausgeht; das geht auch ohne Lizenz und dann anonym. Alternativ: ein
[Issue in diesem Repo](https://github.com/Stacktor/cockpit-releases/issues).

## Warum gibt es hier keinen Quellcode?

Der Quellcode liegt in einem privaten Repo. In diesem hier landen nur die fertigen Installer, die
Update-Informationen und die Prüfsummen.

## Warum kein macOS?

Die Mac-Version lässt sich gerade nicht testen, und ungetestete Installer gebe ich nicht raus.
Sie kommt zurück, sobald sie wieder getestet werden kann. Wer interessiert ist, kann sich bei der
[Alpha-Anmeldung](https://cockpit.mesco.cc/alpha/) auf die Mac-Warteliste setzen.
