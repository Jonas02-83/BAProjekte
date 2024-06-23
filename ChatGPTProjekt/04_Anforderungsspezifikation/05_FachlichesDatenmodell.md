## Fachliches Datenmodell (Author:in)

Erstes: 

Spieler

    Attribute:
        spielerID: Eindeutige Identifikationsnummer des Spielers.
        name: Name des Spielers.
        email: E-Mail-Adresse des Spielers.
        punkte: Aktueller Punktestand des Spielers.
    Beziehungen:
        Ein Spieler kann an mehreren Spielen teilnehmen (1..*).

Spiel

    Attribute:
        spielID: Eindeutige Identifikationsnummer des Spiels.
        status: Aktueller Status des Spiels (z.B. "laufend", "beendet").
        aktuellerSpieler: ID des Spielers, der aktuell am Zug ist.
        spielBreit: Darstellung des Spielbretts.
    Beziehungen:
        Ein Spiel hat mehrere Spieler (4..*).
        Ein Spiel hat mehrere Spielzüge (*).

Spielzug

    Attribute:
        zugID: Eindeutige Identifikationsnummer des Zuges.
        zugNummer: Nummer des Zuges in der Reihenfolge.
        spielerID: ID des Spielers, der den Zug gemacht hat.
        spielfigur: Bezeichnung der Spielfigur, die bewegt wurde.
        feldVon: ID des Startfeldes.
        feldNach: ID des Zielfeldes.
        zugZeit: Zeitstempel des Zuges.
    Beziehungen:
        Ein Spielzug gehört zu einem Spiel (1).
        Ein Spielzug ist einer Spielfigur zugeordnet (1).

Spielfigur

    Attribute:
        figurID: Eindeutige Identifikationsnummer der Spielfigur.
        farbe: Farbe der Spielfigur.
        position: Aktuelle Position der Spielfigur auf dem Spielfeld.
    Beziehungen:
        Eine Spielfigur gehört zu einem Spieler (1).
        Eine Spielfigur steht auf einem Feld (1).

Feld

    Attribute:
        feldID: Eindeutige Identifikationsnummer des Feldes.
        typ: Typ des Feldes (z.B. "Start", "Ziel", "Normal").
        position: Position des Feldes auf dem Spielbrett.
        farbe: Farbe des Feldes.
    Beziehungen:
        Ein Feld kann von einer Spielfigur belegt sein (1).

Chat

    Attribute:
        chatID: Eindeutige Identifikationsnummer der Chatnachricht.
        spielerID: ID des Spielers, der die Nachricht gesendet hat.
        nachricht: Inhalt der Nachricht.
        zeitstempel: Zeitstempel der Nachricht.
    Beziehungen:
        Ein Chatnachricht gehört zu einem Spiel (1).
        Ein Chatnachricht gehört zu einem Spieler (1).
  





Aktuelles (Skizze in Onenote):

User

    Attribute:
        userID: Eindeutige Identifikationsnummer des Nutzers.
        Format: Positive Ganzzahl.
        name: Name des Nutzers.
        Format: String, max. 100 Zeichen.
        email: E-Mail-Adresse des Nutzers.
        Format: String, gültiges E-Mail-Format (z.B., name@example.com), max. 100 Zeichen.
        passwort: Passwort des Nutzers.
        Format: String, min. 8 Zeichen, max. 100 Zeichen.
        punkte: Aktueller Punktestand des Nutzers.
        Format: Positive Ganzzahl.
    Beziehungen:
        Ein User kann an mehreren Spielen als Spieler teilnehmen (1..*).

Spieler

    Attribute:
        spielerID: Eindeutige Identifikationsnummer des Spielers.
        Format: Positive Ganzzahl.
        farbe: Farbe der Spielfiguren des Spielers.
        Format: String, z.B., "Rot", "Blau", "Grün", "Gelb".
    Beziehungen:
        Ein Spieler gehört zu einem User (1).
        Ein Spieler kann an einem Spiel teilnehmen (1..4).

Spiel

    Attribute:
        spielID: Eindeutige Identifikationsnummer des Spiels.
        Format: Positive Ganzzahl.
        status: Aktueller Status des Spiels (z.B., "laufend", "beendet").
        Format: String, max. 20 Zeichen.
        aktuellerSpieler: ID des Spielers, der aktuell am Zug ist.
        Format: Positive Ganzzahl.
        spielBrett: Darstellung des Spielbretts.
        Format: String, JSON-Format zur Beschreibung des Spielbretts.
    Beziehungen:
        Ein Spiel hat 1 bis 4 Spieler (1..4).
        Ein Spiel hat mehrere Spielzüge (*).

Spielzug

    Attribute:
        zugID: Eindeutige Identifikationsnummer des Zuges.
        Format: Positive Ganzzahl.
        zugNummer: Nummer des Zuges in der Reihenfolge.
        Format: Positive Ganzzahl.
        spielerID: ID des Spielers, der den Zug gemacht hat.
        Format: Positive Ganzzahl.
        spielfigur: Bezeichnung der Spielfigur, die bewegt wurde.
        Format: String, z.B., "Figur1", "Figur2".
        feldVon: ID des Startfeldes.
        Format: Positive Ganzzahl.
        feldNach: ID des Zielfeldes.
        Format: Positive Ganzzahl.
        zugZeit: Zeitstempel des Zuges.
        Format: Date, z.B., "YYYY-MM-DD HH:MM".
    Beziehungen:
        Ein Spielzug gehört zu einem Spiel (1).
        Ein Spielzug ist einer Spielfigur zugeordnet (1).

Spielfigur

    Attribute:
        figurID: Eindeutige Identifikationsnummer der Spielfigur.
        Format: Positive Ganzzahl.
        farbe: Farbe der Spielfigur.
        Format: String, z.B., "Rot", "Blau", "Grün", "Gelb".
        position: Aktuelle Position der Spielfigur auf dem Spielfeld.
        Format: Positive Ganzzahl.
    Beziehungen:
        Eine Spielfigur gehört zu einem Spieler (1).
        Eine Spielfigur steht auf einem Feld (1).

Feld

    Attribute:
        feldID: Eindeutige Identifikationsnummer des Feldes.
        Format: Positive Ganzzahl.
        typ: Typ des Feldes (z.B., "Start", "Ziel", "Normal").
        Format: String, max. 20 Zeichen.
        position: Position des Feldes auf dem Spielbrett.
        Format: Positive Ganzzahl.
        farbe: Farbe des Feldes.
        Format: String, z.B., "Rot", "Blau", "Grün", "Gelb".
        belegt: Boolean, ob das Feld derzeit von einer Spielfigur belegt ist.
        Format: Boolean, Werte: true/false.
    Beziehungen:
        Ein Feld kann von einer Spielfigur belegt sein (1).

Chat

    Attribute:
        chatID: Eindeutige Identifikationsnummer der Chatnachricht.
        Format: Positive Ganzzahl.
        spielerID: ID des Spielers, der die Nachricht gesendet hat.
        Format: Positive Ganzzahl.
        nachricht: Inhalt der Nachricht.
        Format: String, max. 500 Zeichen.
        zeitstempel: Zeitstempel der Nachricht.
        Format: Date, z.B., "YYYY-MM-DD HH:MM".
    Beziehungen:
        Eine Chatnachricht gehört zu einem Spiel (1).
        Eine Chatnachricht gehört zu einem Spieler (1).