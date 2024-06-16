# Projekt-Dokumentation

Kamil

| Datum       | Version | Zusammenfassung                                                                 |
| ----------- | ------- | ------------------------------------------------------------------------------- |
| 22/05/2024  | 0.0.1   | Projekt gestartet, Grundstruktur erstellt, Registrierung und Anmeldung implementiert |
| 29/05/2024  | 0.0.2   | Lunch Spots hinzugefügt und Anzeige im Frontend umgesetzt                        |
| 05/06/2024  | 0.0.3   | Check-In-Funktionalität implementiert und Fehlerbehebung                        |
| 12/06/2024  | 1.0.0   | Endgültige Fehlerbehebung und Dokumentation abgeschlossen                       |

## 1 Informieren

### 1.1 Ihr Projekt

Ein Mittagessenplaner, der es Nutzern ermöglicht, sich für verschiedene Orte zum Mittagessen anzumelden und zu sehen, wer sonst noch dort ist.

Das Ziel dieses Projekts ist es, eine Webanwendung zu entwickeln, die verschiedene Mittagessensorte speichert und es Benutzern ermöglicht, sich für ein Datum an einem dieser Orte einzuchecken. Dies hilft den Benutzern, ihre Freunde zu finden und gemeinsam Mittag zu essen. Dabei soll der Umgang mit NoSQL-Datenbanken (MongoDB), Authentifizierung sowie Frontend- und Backend-Entwicklung erlernt und vertieft werden.

### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ        | Beschreibung                                       |
| ---- | --------------- | ---------- | -------------------------------------------------- |
| 1    | Muss            | Funktional | Als Nutzer möchte ich mich registrieren können, um die App zu nutzen. |
| 2    | Muss            | Funktional | Als Nutzer möchte ich mich einloggen können, um Zugang zu meinen Daten zu haben. |
| 3    | Muss            | Funktional | Als Nutzer möchte ich verschiedene Mittagessensorte sehen können, um zu entscheiden, wo ich hingehen möchte. |
| 4    | Muss            | Funktional | Als Nutzer möchte ich mich für einen Mittagessensort an einem bestimmten Datum einchecken können, um meine Anwesenheit zu bestätigen. |
| 5    | Kann            | Funktional | Als Nutzer möchte ich sehen können, wer sich noch an einem bestimmten Mittagessensort eingecheckt hat, um zu wissen, wer dort sein wird. |

### 1.3 Testfälle

| TC-№ | Ausgangslage         | Eingabe                   | Erwartete Ausgabe                                       |
| ---- | -------------------- | ------------------------- | ------------------------------------------------------- |
| 1.1  | Registrierung-Seite  | Nutzerdaten               | Nutzer wird erfolgreich registriert, aber kein `userId` wird zugefügt. |
| 2.1  | Login-Seite          | Nutzername und Passwort   | Nutzer wird erfolgreich eingeloggt und erhält ein Token |
| 3.1  | Hauptseite           | -                         | Liste der Mittagessensorte wird angezeigt               |
| 4.1  | Check-In-Seite       | Auswahl des Ortes und Datum | Check-In schlägt fehl, da kein `userId` vorhanden ist.  |
| 5.1  | Hauptseite           | -                         | Liste der Nutzer, die eingecheckt haben, wird angezeigt |

## 2 Planen

| AP-№ | Frist     | Zuständig | Beschreibung                                              | geplante Zeit |
| ---- | --------- | --------- | --------------------------------------------------------- | ------------- |
| 1.A  | 22/05/2024| Kamil     | Grundstruktur des Projekts erstellen                      | 2 Stunden   |
| 1.B  | 22/05/2024| Kamil     | Registrierung und Login implementieren                    | 4 Stunden     |
| 2.A  | 29/05/2024| Kamil     | Lunch Spots hinzufügen und im Frontend anzeigen           | 4 Stunden     |
| 3.A  | 05/06/2024| Kamil     | Check-In-Funktionalität implementieren                    | 4 Stunden     |
| 4.A  | 12/06/2024| Kamil     | Endgültige Fehlerbehebung und Dokumentation abschliessen   | 4 Stunden     |

Total: 20 Stunden

## 5 Kontrollieren

| TC-№ | Datum      | Resultat                | Tester |
| ---- | ---------- | ----------------------- | ------ |
| 1.1  | 22/05/2024 | Erfolgreich, aber `userId` fehlt | Kamil  |
| 2.1  | 22/05/2024 | Erfolgreich             | Kamil  |
| 3.1  | 29/05/2024 | Erfolgreich             | Kamil  |
| 4.1  | 05/06/2024 | Fehlgeschlagen          | Kamil  |
| 5.1  | 12/06/2024 | Erfolgreich             | Kamil  |

Fazit: Die meisten Testfälle wurden erfolgreich durchgeführt. Ein Problem wurde festgestellt, bei dem während der Registrierung kein `userId` zugefügt wurde, was dazu führte, dass die Check-In-Funktionalität teilweise nicht funktionierte. 
