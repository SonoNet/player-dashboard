# Roadmap: player-dashboard

## Übersicht
Ziel ist es, ein Registrierungssystem für Spieler zu erstellen, bei dem ein Code vom Minecraft-Server erforderlich ist, gefolgt von einer Google-Authentifizierung. Auf dem Dashboard sollen Spielerinformationen wie Name, UUID, Kontostand und Spielzeit angezeigt werden.

1. **Backend-Einrichtung**
2. **Minecraft-Code-Generierung und -Überprüfung**
3. **Google-Authentifizierung und Anmeldung**
4. **Datenbank und Speicherung von Spielerinformationen**
5. **Frontend und Dashboard-Design**
6. **Statistik-Anzeige und Datenabfrage**

---

## Backend-Einrichtung
- [ ] Server-Setup: Erstelle einen Webserver, z. B. mit Node.js oder Django.
- [ ] API-Endpoints: Entwickle APIs für:
  - **Code-Überprüfung** (zum Validieren des Spieler-Codes)
  - **Authentifizierung** (zur Verwaltung der Google-Anmeldung)
  - **Datenabfrage** (für das Dashboard)

---

## Minecraft-Code-Generierung und -Überprüfung
- [ ] **Code-Generierung:** Implementiere ein Minecraft-Plugin oder Skript, das auf den Befehl `/code` reagiert.
  - Generiere zufällige Codes und speichere sie temporär im Server-Backend.
- [ ] **Code-Überprüfung:** Erstelle ein API-Endpoint, das den Code abfragt und überprüft, ob er gültig und noch aktiv ist.

---

## Google-Authentifizierung und Anmeldung
- [ ] **OAuth2-Integration:** Richte Google OAuth2 ein, damit sich Spieler mit ihrem Google-Konto anmelden müssen.
  - Setze dies als Pflichtschritt, nachdem der Code erfolgreich validiert wurde.
- [ ] **Token-Speicherung:** Speichere das Google-Token zur späteren Verifizierung in der Datenbank.

---

## Datenbank und Speicherung von Spielerinformationen
- [ ] **Datenbankstruktur:** Erstelle eine Datenbank für:
  - Spieler-Profile (Name, UUID, Google-ID)
  - Statistiken (Kontostand, Spielzeit usw.)
- [ ] **Datenabfrage:** Implementiere Mechanismen zum Speichern und Abfragen der Daten.

---

## Frontend und Dashboard-Design
- [ ] **Registrierungsseite:** Baue eine Website mit Formularfeldern für:
  - Code-Eingabe
  - Google-Anmeldung
- [ ] **Dashboard:** Erstelle eine Dashboard-Oberfläche, die folgende Informationen anzeigt:
  - Spielername und UUID
  - Kontostand, Spielzeit und andere Statistiken
- [ ] **Benutzerfreundlichkeit:** Implementiere ein modernes, benutzerfreundliches Design.

---

## Statistik-Anzeige und Datenabfrage
- [ ] **Datenintegration:** Binde das Backend so ein, dass die Spielerstatistiken regelmäßig abgefragt und aktualisiert werden.
- [ ] **Kontostand & Spielzeit:** Zeige Statistiken wie Kontostand und Spielzeit auf dem Dashboard.
- [ ] **API-Optimierung:** Stelle sicher, dass die Datenabfrage effizient funktioniert und die Webseite schnell lädt.

---

## Zusatzaufgaben
- [ ] **Sicherheitsprüfung:** Stelle sicher, dass die Registrierung sicher ist und Authentifizierungsdaten verschlüsselt sind.
- [ ] **Fehlerbehebung und Tests:** Teste alle Phasen gründlich und behebe eventuelle Fehler.
- [ ] **Benachrichtigungen:** Füge Benachrichtigungen hinzu (optional), wenn sich Statistiken ändern.
