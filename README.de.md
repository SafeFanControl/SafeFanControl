> [!NOTE]
> Wir nutzen GitHub, um Fehler zu verfolgen, Funktionswünsche zu besprechen und ausführbare Dateien zu veröffentlichen.
> SafeFanControl ist **keine** Open-Source-Software.

<div align="center">

[English](README.md) | [简体中文](README.zh-Hans.md) | [繁體中文](README.zh-Hant.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | **Deutsch** | [Español](README.es.md) | [Français](README.fr.md) | [Русский](README.ru.md)

</div>

---

# SafeFanControl

**Übernimm die Kontrolle über die Lüfter deines Macs**

SafeFanControl ist eine **native macOS-App**, mit der du auf Apple-Silicon- und Intel-Macs Temperaturen überwachen und Lüfterdrehzahlen steuern kannst. Kostenloser Download — deine Lüfter, deine Regeln, und das System bekommt die Kontrolle immer zurück, falls etwas schiefgeht.

[Für macOS herunterladen](https://github.com/SafeFanControl/SafeFanControl/releases)

---

## Funktionen

### Alle Lüftersteuerungsmodi, die du brauchst

SafeFanControl gibt dir die volle Kontrolle darüber, wie dein Mac auf Hitze reagiert – mit drei verschiedenen Betriebsmodi für deinen Arbeitsablauf.

- **Monitor** — Temperaturen und Lüfterdrehzahlen in Echtzeit ablesen, ohne in die Systemsteuerung einzugreifen
- **Safe Max** — fährt automatisch auf volle Drehzahl, sobald ein Temperaturschwellwert erreicht ist, und gibt die Kontrolle an macOS zurück, sobald es sich abkühlt
- **Curve** — definiere eine eigene Temperatur-zu-Drehzahl-Kennlinie für stufenlose, proportionale Steuerung
- Modi sofort über die Menüleiste wechseln — ganz ohne App-Fenster

### Auf Sicherheit ausgelegt

Eine Drei-Prozess-Architektur stellt sicher, dass macOS bei jedem Problem automatisch die Lüftersteuerung zurückerhält – ganz ohne manuelles Eingreifen.

- Ein **Watchdog-Prozess** überwacht den Helfer-Daemon; stürzt er ab, während die Lüfter im manuellen Modus sind, übernimmt macOS sofort
- **Sanfte Überblendungen** verhindern abrupte Drehzahlsprünge, die hörbar oder störend sein könnten
- **Schwellwert-Verriegelung** hält Safe Max bei kurzen Temperaturschwankungen stabil
- Der übliche macOS-Administratordialog installiert den Hintergrund-Helfer — kein Terminal, keine manuellen Schritte

### Immer in der Menüleiste

Eine schlanke Menüleisten-App bringt Live-Sensordaten und Moduswechsel mit einem Klick — immer sichtbar, niemals im Weg.

- CPU- und GPU-Temperaturen werden in Echtzeit aktualisiert
- Aktuelle Lüfterdrehzahl und aktiver Steuerungsmodus stets sichtbar
- Wechsle direkt im Aufklappmenü zwischen Monitor, Safe Max und Curve
- Unterstützt Apple Silicon M1 bis M5 und Intel-Macs mit T2-Chip; in 8 Sprachen verfügbar

---

## Preise

SafeFanControl folgt dem Modell **kostenloser Download, einmaliger Kauf**. Keine Abos. Keine wiederkehrenden Gebühren. Einmal zahlen, für immer besitzen.

| | Kostenlos | Volllizenz |
|---|---|---|
| **Preis** | $0 — für immer | $8.99 — einmalig |
| Monitor-Modus (nur Lesen) | ✅ | ✅ |
| Temperaturanzeige in Echtzeit | ✅ | ✅ |
| Anzeige der Lüfterdrehzahl | ✅ | ✅ |
| CPU-, GPU-, SoC-Sensoren | ✅ | ✅ |
| M1–M5 generationsspezifisch | ✅ | ✅ |
| **Safe-Max-Modus** | ❌ | ✅ |
| **Curve-Modus** | ❌ | ✅ |
| Sanfte Überblendungen | ❌ | ✅ |
| Verriegelung / Sprungunterdrückung | ❌ | ✅ |
| Safe Max mit mehreren Regeln | ❌ | ✅ |
| **Lüftertest-Assistent** | ❌ | ✅ |
| Debug- & Diagnoseseite | ❌ | ✅ |

---

## Download & Installation

### Systemvoraussetzungen

| Voraussetzung | Details |
|---|---|
| **macOS** | 15 (Sequoia) oder neuer |
| **Mac-Hardware** | Apple Silicon (M1, M2, M3, M4, M5) oder Intel-Mac mit T2-Chip |
| **Berechtigungen** | Eine Administrator-Passwortabfrage zur Installation des Hintergrund-Daemons |
| **Speicherplatz** | ~5 MB |

### Installation

1. **Öffne die heruntergeladene `.dmg`** und ziehe SafeFanControl in deinen Programme-Ordner.
2. **Starte die App.** Beim ersten Start installiert ein Administratordialog den Hintergrund-Helfer und den Watchdog-Daemon.
3. **Fertig.** Kein Terminal. Keine manuellen Bestätigungen. Der Lüftertest-Assistent führt dich durch die Prüfung, ob auf deiner Hardware alles funktioniert.

> macOS zeigt beim ersten Start möglicherweise eine Gatekeeper-Meldung an, da die App nicht über den App Store vertrieben wird. **Rechtsklick → Öffnen**, um fortzufahren.

### Deinstallation

SafeFanControl enthält unter **Einstellungen → Deinstallieren** einen vollständigen Deinstallationsvorgang. Er entfernt den Helfer-Daemon, den Watchdog-Daemon und alle zugehörigen Dateien in einem Schritt.

---

## FAQ

**Gibt es eine kostenlose Testphase für die vollen Funktionen?**
Ja — die Modi Safe Max und Curve sind beim ersten Start für eine **14-tägige Testphase** freigeschaltet. Keine Zahlung erforderlich.

**Was deckt die Lizenz ab?**
Eine Lizenz deckt alle deine **privaten** Macs ab. Sie ist nicht für Weiterverbreitung oder gewerblichen Einsatz in Geräteflotten bestimmt.

**Muss ich nach einem macOS-Upgrade erneut kaufen?**
Nein. Deine Lizenz ist dauerhaft.

**Muss ich bei einem neuen Mac erneut kaufen?**
Nein — deine Lizenz gehört dir. Nutze deinen vorhandenen Lizenzschlüssel, um deinen neuen Mac zu registrieren.

**Wie lautet eure Rückerstattungsrichtlinie?**
Da wir deine Privatsphäre respektieren, nutzt die App ein Offline-Registrierungssystem. Einmal ausgestellte Lizenzschlüssel können nicht aus der Ferne deaktiviert werden — daher sind alle Verkäufe endgültig und Standard-Rückerstattungen können nicht gewährt werden. Wir empfehlen dringend, vor dem Kauf die 14-tägige Testphase zu nutzen. Ausnahme: Sollte ein Apple-macOS-Update die zugrunde liegenden Methoden zur Lüftersteuerung dauerhaft deaktivieren, erstatten wir Lizenzen, die in den letzten 30 Tagen gekauft wurden, in voller Höhe.

**Warum ist die App nicht im Mac App Store?**
SafeFanControl installiert einen privilegierten Hintergrund-Daemon, was mit den strengen Sandbox-Regeln des App Store nicht vereinbar ist. Der Vertrieb erfolgt direkt — aber das Installationsprogramm wird über Apples Signatursystem geprüft, notarisiert und signiert.

**Kann ich es nutzen, ohne zu zahlen?**
Ja — der Monitor-Modus ist vollständig kostenlos und bleibt es auch.

**Was passiert, wenn der Lizenzserver in Zukunft offline geht?**
Der Lizenzschlüssel funktioniert offline und erfordert keine Internetprüfung. Du kannst dich jederzeit registrieren, solange du deinen Lizenzschlüssel noch hast.

**Was, wenn du dieses Projekt aufgibst?**
Jedes Produkt hat eine Lebensdauer. Solange ich jedoch programmieren kann und die Einnahmen des Produkts die Grundkosten (etwa die jährliche Gebühr für das Apple Developer Program) decken, werde ich es weiter pflegen. Wenn dir dieses Produkt gefällt, teile es bitte mit deinen Freunden. Wenn (und nur wenn) der Tag kommt, an dem ich dieses Projekt aufgeben muss, werde ich den Quellcode unter der AGPL-v3-Lizenz mit allen zahlenden Nutzern teilen.

**Was, wenn ich meinen Lizenzschlüssel verliere?**
Bitte wende dich an die Verkaufsplattform oder kontaktiere uns direkt.

---

## Datenschutz

SafeFanControl erfasst **keine** Telemetrie, Analysen oder Absturzberichte. Deine Hardware-Daten bleiben auf deinem Gerät.
