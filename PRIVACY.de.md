# TunnelMint-Datenschutzinformationen

Stand: 25. August 2026

Dieses Dokument beschreibt TunnelMint 1.0.0 für macOS.

## Datenverarbeitung

TunnelMint enthält derzeit keine Analysefunktionen, Werbung, Nachverfolgung, Benutzerkonten oder Cloud-Synchronisierung. Die App erfasst und übermittelt keine Nutzungsstatistiken an den Entwickler.

- Metadaten von VPN-Profilen werden lokal auf dem Mac gespeichert.
- Passwörter, Gruppenschlüssel, private Schlüssel und geschützte importierte Konfigurationen werden im macOS-Schlüsselbund gespeichert.
- VPN-Datenverkehr wird lokal durch Apples Network-Extension-Framework und durch den vom Benutzer ausgewählten VPN-Server verarbeitet.
- TunnelMint betreibt den ausgewählten VPN-Server nicht. Die Datenschutz- und Protokollierungsregeln des Serverbetreibers gelten unabhängig davon.
- Ein optionaler Endpunkttest kontaktiert ausschließlich den vom Benutzer ausgewählten Server, um Netzwerk- und TLS-Erreichbarkeit zu prüfen. VPN-Benutzername und Passwort werden dabei nicht übertragen.
- Ausgewählte `.conf`-, `.ovpn`-, `.mobileconfig`-, `.pcf`- und `.pbk`-Dateien werden nur gelesen, wenn der Benutzer sie ausdrücklich importiert.

## Berechtigungen

TunnelMint benötigt die Network-Extension-Berechtigung, um VPN-Tunnel aufzubauen. Wenn „Bei Anmeldung starten“ aktiviert wird, verwaltet macOS TunnelMint außerdem als Anmeldeobjekt. Diese Berechtigungen bleiben in den Systemeinstellungen sichtbar und können dort kontrolliert werden.

## Aufbewahrung und Löschung

Beim Löschen eines Profils entfernt TunnelMint dessen lokal gespeicherte Metadaten und zugehöriges Schlüsselbundmaterial. Benutzer sollten Profile vor der Deinstallation löschen, wenn die App auch die gespeicherten Schlüsselbundeinträge entfernen soll. macOS kann Schlüsselbundeinträge erhalten, wenn nur das App-Bundle gelöscht wird.

## Support- und Datenschutzfragen

Nutze den [öffentlichen Issue-Tracker](https://github.com/LilaQ/TunnelMint-issues/issues) ausschließlich für Fragen ohne vertrauliche Inhalte. Veröffentliche dort keine Zugangsdaten, Schlüssel, Zertifikate, Konfigurationsdateien oder privaten Netzwerkdetails.

Für vertrauliche Sicherheitsmeldungen nutze GitHubs private Meldung von Sicherheitslücken gemäß [SECURITY.md](SECURITY.md). Anbieteridentität und weitere Kontaktdaten, die für einen Store oder ein Vertriebsgebiet erforderlich sind, werden im jeweiligen Store-Eintrag veröffentlicht.
