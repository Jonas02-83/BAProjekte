# Projekthandbuch *`<`Projektname`>`* {-}

## Historie
| Version | Status | Datum | Autor(en) | Erläuterung |
| --- | --- | --- | --- | --- | 
| 0.1 | In Arbeit | `<`17.06.2024`>` | `<`ChatGPT`>` | `<`Mit ChatGPT geschriebene Abschnitte`>` | 
| ... | ... | ... | ...	| ... | 

## Zusammenfassung

Dieses Projekthandbuch beschreibt die Planung, Durchführung und Kontrolle der Entwicklung eines digitalen "Mensch ärgere 
dich nicht"-Spiels als JavaFX-Anwendung, einschließlich Server-Client-Kommunikation über RMI, mit besonderem Fokus auf 
Risikomanagement und regelmäßigen Feedback-Schleifen.

## Einleitung

Zuerst wird der Zweck des Dokuments vorgestellt. Im Anschluss wird der redaktionelle Prozess erläutert und wer bei 
Änderungen informiert werden muss.

###	Zweck des Dokuments 

Dieses Projekthandbuch dient als zentrale Informationsquelle für alle Beteiligten des Projekts "Digitales 'Mensch ärgere 
dich nicht'-Spiel". Es enthält alle relevanten Informationen zur Planung, Entwicklung und Durchführung des Projekts. Ziel 
ist es, die Struktur und den Ablauf des Projekts klar zu definieren und sicherzustellen, dass alle Teammitglieder über den 
aktuellen Stand und die nächsten Schritte informiert sind. Das Handbuch soll als Nachschlagewerk dienen, um die Kommunikation 
zu erleichtern und die Qualität der Projektergebnisse zu sichern.

###	Redaktion

Für die Erstellung und Pflege dieses Projekthandbuchs ist die Projektleiterin, Frau Schmidt, verantwortlich. Sie stellt sicher, 
dass alle Informationen aktuell und vollständig sind und dass notwendige Änderungen zeitnah eingearbeitet werden.

###	Verteiler

Alle Änderungen und Aktualisierungen des Projekthandbuchs werden dem gesamten Projektteam mitgeteilt. Dies umfasst:

- Frau Schmidt (Projektleiterin)
- Herr Schneider (Anforderungsanalyst und fachlicher Chefdesigner)
- Frau Fischer (Systemarchitektin)
- Herr Becker (Testmanager)

Die Benachrichtigung erfolgt über eine entsprechende Nachricht im dedizierten Discord-Channel des Projekts. Dies gewährleistet, 
dass alle Teammitglieder stets über den aktuellen Stand und eventuelle Anpassungen informiert sind.

## Projektdefinition

### Vorgeschichte 

Das Projekt "Digitales 'Mensch ärgere dich nicht'-Spiel" wurde initiiert durch Herrn Müller, der die Idee hatte, das klassische Brettspiel in eine digitale Form zu übertragen. Herr Müller wandte sich an unser Entwicklerteam mit dem Wunsch, ein Spiel zu entwickeln, das sowohl den traditionellen Charme des Brettspiels beibehält als auch moderne, digitale Features integriert. In einem ersten Gespräch wurden die grundlegenden Anforderungen und Ziele des Projekts besprochen. Dabei stellte sich heraus, dass Herr Müller eine JavaFX-Anwendung bevorzugt, die sowohl Einzel- als auch Mehrspielermodi unterstützt. Der Kommunikationsweg zwischen Client und Server soll über Java RMI realisiert werden.

###	Inhaltliche Kurzdarstellung

Das Ziel des Projekts ist die Entwicklung eines digitalen "Mensch ärgere dich nicht"-Spiels, das als JavaFX-Anwendung auf Computern läuft. 
Die Hauptfunktionen des Spiels umfassen:

- Server-Client-Architektur: Das Spiel wird als Server-Client-Anwendung implementiert, wobei die Kommunikation über Java RMI erfolgt.
- Spielmodi: Es wird sowohl einen Einzelspielermodus gegen KI-Gegner als auch einen Mehrspielermodus geben, in dem Spieler online gegen Freunde oder zufällige Gegner antreten können.
- Teilnehmeranzahl: Bis zu vier Spieler können gleichzeitig an einem Spiel teilnehmen, analog zum klassischen Brettspiel.
- Design: Das Spiel wird ein klassisches Design mit einer modernen, ansprechenden Benutzeroberfläche haben, um sowohl Nostalgie als auch zeitgemäße Optik zu bieten.
- Zusatzfunktionen: Zu den zusätzlichen Funktionen gehören ein In-Game-Chat für die Spielerkommunikation, ein Punktesystem zur Erhöhung der Motivation und einfache, ansprechende    Animationen.

Das Projekt soll innerhalb eines Zeitrahmens von sechs Monaten realisiert werden, wobei regelmäßige Feedback-Schleifen und Meetings eingeplant sind, um den Fortschritt zu besprechen und notwendige Anpassungen vorzunehmen.

###	Vertragsbasis

Das Projekt wird im Rahmen des Moduls „Secure Software Engineering“ erstellt. Es gelten die folgenden Rahmenbedingungen:

...

> Hinweis: Normalerweise sind hier die Verweise auf die Verträge hinterlegt. In den Verträgen ist die genaue Leistung 
> festgehalten. Hier stehen auch die zeitlichen Rahmenbedingungen, die Verpflichtungen der Vertragspartner, 
> Gewährleistungen und Strafen bei einer Vertragsverletzung.

###	Projektergebnis

...

###	Informelle Ziele des Projektes

Die Projektbeteiligten sollen den Software Engineering Prozess und die wichtigsten Produkte der Softwareerstellung 
kennenlernen.

### Sonstige Besonderheiten

##	Risiken, besondere Rahmenbedingungen

Die Risiken und Maßnahmen finden sich in der Datei Risikoliste im Ordner 03_Risikoliste.

##	Projektorganisation

###	Teamaufbau

| Name | Rolle | Erreichbarkeit |
| --- | --- |  --- |
| ... | ... | ... |  

> Hinweis: Hier kann auch auf externe Organigramme verwiesen werden.

...

### Zusammenarbeit mit dem Kunden 

> **Hinweis:** im Praktikum wird der Kunde bzw. die Kundin durch den Betreuer bzw. die Betreuerin vertreten.

...

### Besprechungen

...

## Planungen

### Projektplan und Meilensteine

> **Inhalt:** enthält normalerweise einen Verweis auf den Projektplan, z.B. auf eine externe Datei eines externen
> Projektplanungstools. 

> **Hinweis:** wegen der kurzen Laufzeit des Projekts wird auf eine aufwendigere Projektplanung verzichtet. Die
> Aufgabenpakete werden jeweils bei den wöchentlichen Besprechungen verteilt und in den Besprechungsprotokollen 
> dokumentiert. 

...

### Restaufwandschätzung

> **Inhalt:** enthält normalerweise ein Verweis auf eine externe Datei oder auf eine externe Anwendung mit der die
> Aufwände kontrolliert werden. Dazu müssen die geleisteten Aufwände und die Restaufwände möglichst wöchentlich 
> überprüft werden, damit die Kosten für das Projekt nicht aus dem Ruder laufen. Normalerweise wird dazu von jedem
> Teammitglied eine Mitteilung über die wöchentlich geleisteten Aufwände und die Restaufwandschätzung für die 
> aktuellen Aufgaben verlangt. 

## Qualitätssicherung

> **Inhalt:** enthält normalerweise einen Verweis auf ein externes Dokument, das Qualitätssicherungshandbuch. 
> Das Qualitätssicherungshandbuch richtet sich an alle Teammitglied und soll ein gemeinsames Verständnis für die 
> Aktivitäten schaffen, die durchzuführen sind, damit qualitativ hochwertige Produkte entstehen. Das 
> Qualitätssicherungshandbuch dokumentiert die sachgerechte Anwendung der Qualitätssicherungsmaßnahmen (QS-Maßnahmen) 
> und berücksichtigt die firmeneigenen und die Qualitätsanforderung des Kunden. Die im Qualitätssicherungshandbuch 
> dokumentierten QS-Maßnahmen müssen im Projektplan berücksichtigt werden.  
> Das Qualitätssicherungshandbuch wird vom Qualitätsbeauftragten in Absprache mit dem Projektleiter geschrieben.

> **Hinweis:** in unserem Projekt entfällt die Rolle des Qualitätsbeauftragten.

## Datenschutz

> Hinweis: Dokumentation der Datenschutzrichtlinien, die für dieses Projekt relevant sind. Hier könnte z.B. auch ein 
> Hinweis auf einen Geheimhaltungsvertrag stehen, der für dieses Projekt gilt und von Mitarbeiter:innen unterschrieben 
> werden muss.

## Dokumentation und Ablage

Im gesamten Projektverlauf ist auf eine saubere und konsistente Ablage aller erstellten Produkte und relevanten 
Dokumente zu achten.

...

## Referenzliste

> Hinweis: Verweis auf alle sonstigen existierenden Dokumente, die mit der Projektabwicklung in Zusammenhang stehen.

## Abkürzungsverzeichnis un Glossar

> Hinweis: Erläuterung spezieller Abkürzungen und wichtigster Begriffe
