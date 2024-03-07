# Esercizio di oggi: Primo DB

nome repo: db-first

Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

## Svolgimento

Dati da raccogliere:

- id
- modello
- marca
- anno di produzione
- km percorsi
- ultima revisione
- incidenti subiti
- precedente possessore
- posteggio
- cambio
- carburante
- prezzo
- trazione
- equipaggiamento
- tipo di carrozzeria
- potenza
- numero di portiere
- numero sedili
- colore

## Tabella DB

| FIELD           | TYPE         | ATTRIBUTES                         | INDEXES     |
| --------------- | ------------ | ---------------------------------- | ----------- |
| id              | INT          | NOT NULL, UNSIGNED, AUTO INCREMENT | PRIMARY KEY |
| modello         | VARCHAR(50)  | NOT NULL                           |             |
| marca           | VARCHAR(20)  | NOT NULL                           |             |
| annoProduzione  | YEAR         | NOT NULL                           |             |
| kmPercorsi      | MEDIUMINT    | NOT NULL, DEFAULT(0)               |             |
| ultimaRevisione | DATE         | NULL                               |             |
| incidentiSubiti | TINYINT      | NULL                               |             |
| prePossessore   | VARCHAR(50)  | NOT NULL, DEFAULT(anonimo)         |             |
| posteggio       | VARCHAR(10)  | NOT NULL                           |             |
| cambio          | VARCHAR(10)  | NOT NULL, DEFAULT(maunuale)        |             |
| carburante      | VARCHAR(20)  | NOT NULL, DEFAULT(benzina)         |             |
| prezzo          | MEDIUMINT    | NOT NULL                           |             |
| trazione        | VARCHAR(20)  | NOT NULL, DEFAULT(anteriore)       |             |
| carrozzeria     | VARCHAR(20)  | NOT NULL                           |             |
| potenza         | SMALLINT     | NOT NULL                           |             |
| nPortiere       | TINYINT      | NOT NULL                           |             |
| nSedili         | TINYINT      | NOT NULL                           |             |
| colore          | VARCHART(30) | NOT NULL                           |             |
