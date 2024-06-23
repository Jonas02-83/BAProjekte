##	Nichtfunktionale Anforderungen	

### Nichtfunktionale Anforderungen und Tests

1. **Leistungsanforderungen:**
   - **Anforderung:** Das System muss in der Lage sein, maximal 1000 gleichzeitige Benutzer ohne merkliche Leistungsverschlechterung zu unterstützen.
   - **Test:** Durchführung eines Lasttests, bei dem 1000 Benutzer gleichzeitig auf das System zugreifen und verschiedene Aktionen ausführen (z.B. Anmelden, Spiel erstellen, Spiel beitreten). Es wird überprüft, ob die Antwortzeit des Systems unter 2 Sekunden bleibt.

2. **Zuverlässigkeit und Verfügbarkeit:**
   - **Anforderung:** Das System muss eine Verfügbarkeit von 99,9 % pro Jahr gewährleisten.
   - **Test:** Überwachung des Systems über einen Zeitraum von 30 Tagen. Ausfallzeiten werden protokolliert und die Verfügbarkeit wird berechnet. Die erwartete Ausfallzeit darf nicht mehr als 43,2 Minuten pro Monat betragen.

3. **Sicherheit:**
   - **Anforderung:** Das System muss sicherstellen, dass alle Datenübertragungen zwischen Client und Server verschlüsselt sind.
   - **Test:** Durchführung eines Penetrationstests, bei dem überprüft wird, ob die Datenübertragung mit TLS verschlüsselt ist. Überprüfung der Verschlüsselung mittels Netzwerk-Sniffer-Tools wie Wireshark.

4. **Benutzbarkeit:**
   - **Anforderung:** Der Benutzer muss in der Lage sein, alle Hauptfunktionen (Anmelden, Registrieren, Spiel erstellen, Spiel beitreten) ohne Schulung oder externe Hilfe zu nutzen.
   - **Test:** Durchführung eines Usability-Tests mit 10 Testpersonen, die die Hauptfunktionen ohne vorherige Einweisung nutzen. Es wird gemessen, wie viele der Testpersonen die Aufgaben ohne Unterstützung erfolgreich abschließen.

5. **Wartbarkeit:**
   - **Anforderung:** Der Code des Systems muss modular aufgebaut und gut dokumentiert sein, sodass Änderungen und Erweiterungen leicht vorgenommen werden können.
   - **Test:** Eine unabhängige Gruppe von Entwicklern erhält die Aufgabe, eine kleine Änderung oder Erweiterung im System vorzunehmen. Es wird überprüft, ob sie dies innerhalb von 2 Stunden erledigen können, wobei keine vorherige Kenntnis des Codes vorausgesetzt wird.

6. **Portabilität:**
   - **Anforderung:** Das System muss auf den Betriebssystemen Windows, macOS und Linux lauffähig sein.
   - **Test:** Installation und Ausführung des Systems auf den drei genannten Betriebssystemen. Überprüfung, ob alle Funktionen wie erwartet arbeiten und keine Betriebssystemspezifischen Fehler auftreten.

7. **Effizienz:**
   - **Anforderung:** Das System muss eine durchschnittliche CPU-Auslastung von weniger als 50% und eine Speicherauslastung von weniger als 200 MB auf einem Standard-Desktop-Computer gewährleisten.
   - **Test:** Monitoring der CPU- und Speicherauslastung während der normalen Nutzung des Systems über einen Zeitraum von 8 Stunden. Überprüfung, ob die gemessenen Werte innerhalb der geforderten Grenzen bleiben.

### Zusammenfassung

Die nichtfunktionalen Anforderungen beschreiben die Qualitätsmerkmale des Systems, die nicht direkt mit spezifischen Funktionen verbunden sind, aber für die Gesamtleistung und Benutzererfahrung wichtig sind. Die zugehörigen Tests stellen sicher, dass diese Anforderungen erfüllt werden, indem sie unter realistischen Bedingungen überprüft werden.
