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
        name: Name des Nutzers.
        email: E-Mail-Adresse des Nutzers.
        passwort: Passwort des Nutzers.
        punkte: Aktueller Punktestand des Nutzers.
    Beziehungen:
        Ein User kann an mehreren Spielen als Spieler teilnehmen (1..*).

Spieler

    Attribute:
        spielerID: Eindeutige Identifikationsnummer des Spielers.
        farbe: Farbe der Spielfiguren des Spielers.
    Beziehungen:
        Ein Spieler gehört zu einem User (1).
        Ein Spieler kann an einem Spiel teilnehmen (1..4).

Spiel

    Attribute:
        spielID: Eindeutige Identifikationsnummer des Spiels.
        status: Aktueller Status des Spiels (z.B. "laufend", "beendet").
        aktuellerSpieler: ID des Spielers, der aktuell am Zug ist.
        spielBrett: Darstellung des Spielbretts.
    Beziehungen:
        Ein Spiel hat 1 bis 4 Spieler (1..4).
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
        belegt: Boolean, ob das Feld derzeit von einer Spielfigur belegt ist.
    Beziehungen:
        Ein Feld kann von einer Spielfigur belegt sein (1).

Chat

    Attribute:
        chatID: Eindeutige Identifikationsnummer der Chatnachricht.
        spielerID: ID des Spielers, der die Nachricht gesendet hat.
        nachricht: Inhalt der Nachricht.
        zeitstempel: Zeitstempel der Nachricht.
    Beziehungen:
        Eine Chatnachricht gehört zu einem Spiel (1).
        Eine Chatnachricht gehört zu einem Spieler (1).