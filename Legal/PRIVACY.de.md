# Datenschutzrichtlinie für Quick Paste History

**Letzte Aktualisierung: 8. Mai 2026**

---

## 1. Erfassung und Nutzung von Informationen

Quick Paste History ist ein Zwischenablage-Verwaltungstool, dessen Kernfunktion darin besteht, Zwischenablageinhalte lokal auf Ihrem Gerät aufzuzeichnen, zu verwalten und abzurufen.

### 1.1 Informationen, die wir **nicht** erfassen

- Persönliche Identifikationsinformationen (Name, Ausweisnummer, Adresse usw.)
- Sensible Informationen wie Kontopasswörter, Bankkartennummern usw.
- Gerätekennungen (IDFV, IDFA usw.)
- Browserverlauf, Standortinformationen
- Kontakte, Fotoalbum, Mikrofon, Kameradaten
- Nutzungsverhaltensstatistiken oder Analysedaten

### 1.2 Informationen, auf die wir **zugreifen**

Quick Paste History greift nur auf die folgenden Informationen lokal auf Ihrem Gerät zu, die für seine Kernfunktionen erforderlich sind:

| Datentyp | Zweck | Hochladen auf Server |
|----------|-------|:-------------------:|
| **Zwischenablage-Inhalt** | Zeichnet vom Benutzer kopierten Text/Links auf, unterstützt Suche, Favoriten und Schnellbefüllung | Nur lokale Speicherung |
| **iCloud** | Synchronisiert den Verlauf über NSUbiquitousKeyValueStore zwischen Ihren Geräten | Nur iCloud-private Synchronisation |
| **App Store In-App-Kauf** | Überprüft den Kaufstatus der Pro-Funktionen (nur Quittungsprüfung) | Keine Kaufdetails erfasst |

> Die gesamte Verarbeitung von Zwischenablagedaten erfolgt lokal auf dem Gerät und **wird nicht auf einen externen Server hochgeladen**.

---

## 2. Datenspeicherung

### 2.1 Lokale Speicherung

- Zwischenablage-Verläufe werden in einer SwiftData-Datenbank innerhalb des App-Sandbox gespeichert
- Die Datenbank ist nicht verschlüsselt (der Apple-Sandbox-Mechanismus bietet Systemebenen-Isolation)
- Benutzer können den gesamten Verlauf manuell löschen

### 2.2 iCloud-Synchronisation (Optionale Funktion)

- Nach Aktivierung wird der Verlauf über `NSUbiquitousKeyValueStore` in Ihrem eigenen iCloud-Konto synchronisiert
- Die Daten sind durch iCloud-Sicherheitsmechanismen geschützt und für den Entwickler nicht zugänglich
- Die Synchronisation kann jederzeit in den Einstellungen deaktiviert werden
- Das Deaktivieren der Synchronisation löscht keine lokalen Daten

### 2.3 Datenaufbewahrung

- Der Verlauf wird standardmäßig aufbewahrt; Benutzer können einzelne Einträge manuell löschen oder alles löschen
- Löschvorgänge treten sofort in Kraft und sind nicht umkehrbar

---

## 3. Datenweitergabe

Quick Paste History **gibt keine Benutzerdaten an Dritte weiter**, einschließlich, aber nicht beschränkt auf:

- Verkauft keine Benutzerdaten
- Verwendet keine Daten für Werbung oder Benutzerprofilierung
- Sendet keine Zwischenablageinhalte an Drittanbieter-APIs
- Bindet keine Analyse-SDKs von Drittanbietern ein

---

## 4. Tastaturerweiterung und Berechtigungen

Quick Paste History bietet eine Tastaturerweiterung (Keyboard Extension) zum schnellen Einfügen von Verlaufsinhalten in jeder App:

- **Zugriff**: Die Tastaturerweiterung läuft nur, wenn sie aktiviert ist, und liest nur Zwischenablageinhalte
- **Netzwerk**: Die Tastaturerweiterung hat keine Netzwerkzugriffsberechtigung
- **Datenisolierung**: Die Tastaturerweiterung teilt sich Sandbox-Daten mit der Haupt-App, gibt sie jedoch nicht nach außen frei

---

## 5. Lesen der Zwischenablage

Quick Paste History liest die Zwischenablage in folgenden Situationen:
- Wenn die App im Vordergrund läuft, erkennt sie Änderungen der Zwischenablage und zeichnet neue Inhalte auf
- Wenn der Benutzer aktiv Inhalte mit Quick Paste History teilt

Gemäß den iOS-Systemanforderungen löst das erste Lesen der Zwischenablage eine systemweite Berechtigungsabfrage aus. Benutzer können diese Berechtigung jederzeit in den Systemeinstellungen verwalten.

---

## 6. Datenschutz von Kindern

Quick Paste History erhebt keine personenbezogenen Daten von Kindern.

---

## 7. Änderungen der Datenschutzrichtlinie

Wenn sich die Datenschutzrichtlinie ändert, aktualisieren wir das Datum der „Letzten Aktualisierung" oben auf der Seite und informieren die Benutzer über In-App-Ankündigungen oder Versionsaktualisierungshinweise.

---

## 8. Kontakt

Bei Fragen zur Datenschutzrichtlinie kontaktieren Sie uns bitte über die folgenden Kanäle:

- **Entwickler**: 陈修
- **E-Mail**: chensingyou@126.com
- **App**: Quick Paste History (Entwickler: Singyou)

---

> **Zusammenfassung: Ihre Daten gehören Ihnen.** Quick Paste History lädt keine Inhalte auf Server hoch, verfolgt kein Benutzerverhalten und bindet keine SDKs von Drittanbietern ein. Alle Zwischenablagedaten werden nur lokal auf dem Gerät und im privaten iCloud-Bereich verarbeitet.
