## Systemübersicht (Author:in)

Die Systemarchitektur des digitalen "Mensch ärgere dich nicht"-Spiels basiert auf einer Client-Server-Architektur. Im Folgenden wird ein grober Überblick über die erwartete Systemarchitektur gegeben:

- Client-Anwendung: Die Client-Anwendung wird als JavaFX-Anwendung realisiert und stellt die Benutzeroberfläche des Spiels dar. Sie kommuniziert mit dem Server über Remote Method Invocation (RMI) und ist für die Darstellung des Spielbretts, der Spielfiguren und der Benutzereingaben verantwortlich.
- Server-Anwendung: Die Server-Anwendung ist für die Verwaltung der Spiele, die Authentifizierung der Benutzer und die Bereitstellung der Spielregeln zuständig. Sie kommuniziert mit den Clients über RMI und verwaltet die Spielzustände, die Spielergebnisse und die Chat-Nachrichten.
- Datenbank: Die Datenbank speichert die Benutzerdaten, die Spielergebnisse und die Chat-Nachrichten. Sie wird von der Server-Anwendung verwendet, um die Daten persistent zu speichern und bei Bedarf abzurufen.
- Schnittstellen zu Nachbarsystemen: Falls Schnittstellen zu Nachbarsystemen bestehen, müssen diese in die Systemarchitektur integriert werden. Beispielsweise könnte eine Schnittstelle zu einem externen Authentifizierungssystem oder einem Zahlungssystem erforderlich sein. Diese Schnittstellen müssen in der Systemarchitektur abgebildet und dokumentiert werden.

Die folgende Abbildung zeigt die erwartete Systemarchitektur des digitalen "Mensch ärgere dich nicht"-Spiels:

Die Abbildung der Systemarchitektur sollte die folgenden Komponenten und Beziehungen enthalten:

- Client-Anwendung: Die Client-Anwendung sollte als eigenständiger Block dargestellt werden. Sie kann mit einem Symbol für eine JavaFX-Anwendung oder einem anderen passenden Symbol gekennzeichnet werden.
- Server-Anwendung: Die Server-Anwendung sollte als eigenständiger Block dargestellt werden. Sie kann mit einem Symbol für eine Server-Anwendung oder einem anderen passenden Symbol gekennzeichnet werden.
- Datenbank: Die Datenbank sollte als eigenständiger Block dargestellt werden. Sie kann mit einem Symbol für eine Datenbank oder einem anderen passenden Symbol gekennzeichnet werden.
- Schnittstellen zu Nachbarsystemen: Falls Schnittstellen zu Nachbarsystemen bestehen, sollten diese als Linien zwischen den entsprechenden Komponenten dargestellt werden. Jede Linie sollte mit einer Beschriftung versehen werden, die die Art der Schnittstelle und die beteiligten Komponenten beschreibt.
- Beziehungen: Die Beziehungen zwischen den Komponenten sollten durch Linien dargestellt werden. Die Linien können mit Pfeilen versehen werden, um die Richtung der Kommunikation anzuzeigen. Jede Linie sollte mit einer Beschriftung versehen werden, die die Art der Beziehung beschreibt (z.B. RMI-Kommunikation zwischen Client und Server).

Beziehungen:

Die Beziehung zwischen der Client-Anwendung, der Server-Anwendung und der Datenbank kann wie folgt beschrieben werden:

- Client-Anwendung und Server-Anwendung: Die Client-Anwendung kommuniziert mit der Server-Anwendung über Remote Method Invocation (RMI). Die Client-Anwendung sendet Anfragen an die Server-Anwendung, um Spiele zu starten, Züge auszuführen oder Chat-Nachrichten zu senden. Die Server-Anwendung verarbeitet die Anfragen und sendet die entsprechenden Antworten an die Client-Anwendung zurück.
- Server-Anwendung und Datenbank: Die Server-Anwendung kommuniziert mit der Datenbank, um Benutzerdaten, Spielergebnisse und Chat-Nachrichten zu speichern und abzurufen. Die Server-Anwendung sendet SQL-Anfragen an die Datenbank, um Daten zu lesen oder zu schreiben. Die Datenbank verarbeitet die Anfragen und sendet die entsprechenden Antworten an die Server-Anwendung zurück.
- Client-Anwendung und Datenbank: Die Client-Anwendung kommuniziert nicht direkt mit der Datenbank. Stattdessen werden alle Anfragen und Antworten über die Server-Anwendung geleitet. Die Client-Anwendung sendet Anfragen an die Server-Anwendung, die dann die entsprechenden SQL-Anfragen an die Datenbank sendet und die Antworten an die Client-Anwendung zurücksendet.
