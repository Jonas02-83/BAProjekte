## Fachliches Datenmodell (Author:in)

Erstes: 

Entitätstypen:

    Spieler: Der Entitätstyp Spieler beschreibt die Eigenschaften eines Spielers im Spiel. Ein Spieler hat eine eindeutige ID, einen Benutzernamen, ein Passwort und eine E-Mail-Adresse. Ein Spieler kann an einem oder mehreren Spielen teilnehmen.
    Spiel: Der Entitätstyp Spiel beschreibt die Eigenschaften eines Spiels. Ein Spiel hat eine eindeutige ID, einen Namen, ein Datum und eine Uhrzeit, an dem es stattfindet, und eine maximale Anzahl von Spielern. Ein Spiel kann von einem oder mehreren Spielern gespielt werden.
    Spielfigur: Der Entitätstyp Spielfigur beschreibt die Eigenschaften einer Spielfigur im Spiel. Eine Spielfigur hat eine eindeutige ID, eine Farbe und eine Position auf dem Spielbrett. Eine Spielfigur gehört zu genau einem Spieler und kann an einem oder mehreren Spielen teilnehmen.
    Chat-Nachricht: Der Entitätstyp Chat-Nachricht beschreibt die Eigenschaften einer Chat-Nachricht im Spiel. Eine Chat-Nachricht hat eine eindeutige ID, einen Text, ein Datum und eine Uhrzeit, zu der sie gesendet wurde, und einen Absender. Eine Chat-Nachricht gehört zu genau einem Spiel.

Beziehungen:

    Spieler - Spiel (n): Ein Spieler kann an einem oder mehreren Spielen teilnehmen. Ein Spiel kann von einem oder mehreren Spielern gespielt werden.
    Spieler - Spielfigur (1): Ein Spieler kann eine oder mehrere Spielfiguren besitzen. Eine Spielfigur gehört zu genau einem Spieler.
    Spiel - Spielfigur (n): Ein Spiel kann eine oder mehrere Spielfiguren enthalten. Eine Spielfigur kann an einem oder mehreren Spielen teilnehmen.
    Spiel - Chat-Nachricht (1): Ein Spiel kann eine oder mehrere Chat-Nachrichten enthalten. Eine Chat-Nachricht gehört zu genau einem Spiel.

Einschränkungen:

    Die E-Mail-Adresse eines Spielers muss eindeutig sein.
    Das Passwort eines Spielers muss mindestens 8 Zeichen lang sein und mindestens eine Zahl, einen Großbuchstaben und ein Sonderzeichen enthalten.
    Die maximale Anzahl von Spielern pro Spiel beträgt 4.
    Die Position einer Spielfigur auf dem Spielbrett muss gültig sein (d.h. innerhalb der Grenzen des Spielbretts und nicht auf einer Position, die bereits von einer anderen Spielfigur besetzt ist)






  
