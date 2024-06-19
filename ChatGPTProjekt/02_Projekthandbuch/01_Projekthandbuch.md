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

Dieses Projekthandbuch dient als zentrale Referenz für alle Aspekte der Entwicklung des digitalen "Mensch ärgere dich 
nicht"-Spiels. Es stellt sicher, dass alle Teammitglieder und Stakeholder über die Ziele, Anforderungen, Meilensteine und 
Prozesse des Projekts informiert sind. Das Dokument soll Transparenz schaffen und die Kommunikation zwischen allen 
Beteiligten erleichtern, indem es klare Richtlinien und Verantwortlichkeiten festlegt. Zudem dient es als Nachschlagewerk 
für alle technischen und organisatorischen Details des Projekts.

###	Redaktion

Die Verantwortung für die Erstellung, Pflege und Aktualisierung dieses Projekthandbuchs liegt beim Projektleiter. Der Projektleiter ist dafür verantwortlich, dass das Dokument stets aktuell ist und alle relevanten Informationen enthält. Bei Fragen oder Anmerkungen zum Projekthandbuch steht der Projektleiter als Ansprechpartner zur Verfügung.  

###	Verteiler

Über Änderungen am Projekthandbuch wird das gesamte Projektteam informiert. Änderungen werden im Discord-Channel des Projekts bekannt gegeben, um sicherzustellen, dass alle Teammitglieder zeitnah über Neuerungen und Anpassungen informiert sind. Der Verteiler umfasst die folgenden Personen:

- Frau Schmidt (Projektleiterin)
- Herr Schneider (Anforderungsanalyst und Chefdesigner)
- Frau Fischer (Systemarchitektin)
- Herr Becker (Testmanager)

Durch diese Vorgehensweise wird gewährleistet, dass alle relevanten Informationen und Änderungen transparent kommuniziert werden und das Projektteam stets auf dem neuesten Stand ist.

## Projektdefinition

### Vorgeschichte 

Das digitale "Mensch ärgere dich nicht"-Spielprojekt wurde initiiert, als Herr Müller, ein interessierter Kunde, unsere 
Entwicklerfirma kontaktierte. Herr Müller hatte den Wunsch, das klassische Brettspiel "Mensch ärgere dich nicht" in eine 
moderne, digitale Form zu bringen. Sein Ziel war es, eine Anwendung zu entwickeln, die das traditionelle Spielerlebnis auf 
den Computer überträgt und dabei sowohl Einzel- als auch Mehrspielermodi bietet. Nachdem Herr Müller seine Anforderungen und 
Vorstellungen in einem ersten Gespräch mit Frau Schmidt, der Projektleiterin, erläutert hatte, wurde beschlossen, das 
Projekt zu starten und die Planung und Umsetzung in Angriff zu nehmen.

Die ursprüngliche Idee entstand aus Herrn Müllers persönlichem Interesse an Brettspielen und seiner Vision, diese auch 
digital zu erleben und mit anderen Spielern weltweit teilen zu können. Durch das Einbinden moderner Technologien und die 
Nutzung von JavaFX für die Benutzeroberfläche sowie RMI für die Server-Client-Kommunikation soll ein authentisches und 
dennoch zeitgemäßes Spielerlebnis geschaffen werden.

###	Inhaltliche Kurzdarstellung

Das digitale "Mensch ärgere dich nicht"-Spielprojekt zielt darauf ab, eine JavaFX-basierte Anwendung zu entwickeln, die das 
klassische Brettspiel auf den Computer bringt. Die Anwendung wird als Server-Client-Applikation realisiert, wobei die 
Kommunikation über RMI (Remote Method Invocation) erfolgt. Das Spiel wird sowohl Einzelspieler- als auch Mehrspielermodi 
unterstützen. Im Einzelspielermodus können Spieler gegen KI-Gegner antreten, während im Mehrspielermodus Spiele gegen 
Freunde oder zufällige Gegner online möglich sind. Bis zu vier Spieler können gleichzeitig an einem Spiel teilnehmen.

Das Design des Spiels wird eine klassische Ästhetik mit einer modernen Benutzeroberfläche kombinieren, um die Nostalgie des 
traditionellen Spiels zu bewahren und gleichzeitig ein ansprechendes digitales Erlebnis zu bieten. Zu den wesentlichen 
Features gehören eine Chat-Funktion für die Kommunikation während des Spiels, ein Punktesystem zur Steigerung der Motivation 
und einfache, aber ansprechende Animationen.

Das Projekt wird über einen Zeitraum von sechs Monaten realisiert und umfasst regelmäßige Feedback-Schleifen, um 
sicherzustellen, dass die Anforderungen des Kunden erfüllt und notwendige Anpassungen zeitnah vorgenommen werden können. Ein 
detaillierter Projektplan wird erstellt, der alle Funktionen und Meilensteine definiert, um eine strukturierte und 
zielgerichtete Entwicklung zu gewährleisten.

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
