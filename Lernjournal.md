# M164 - Datenbanken erstellen und Daten einfügen
## Lernjournal & Kursübersicht

---

## Quellen & Ressourcen

**TBZ:**
- [Harald Müller's Aktuelle Kurse](https://gitlab.com/harald.mueller/aktuelle.kurse/-/tree/master/m164)
- [TBZ Studenten Repository](https://gitlab.com/ch-tbz-it/Stud/m164/)

**Sonstige:**
- [Modulbaukasten](https://www.modulbaukasten.ch/module/164/1/de-DE?title=Datenbanken-erstellen-und-Daten-einf%C3%BCgen)
- [Datenbank Grundlagen - Beziehungen](https://www.datenbank-grundlagen.de/beziehungen-datenbanken.html)
- [Informatikzentrale - SELECT Klauseln Merksatz](https://www.informatikzentrale.de/select-klauseln-merksatz.html)

---

## Leistungsbeurteilungen (Prüfungen)

### Lernportfolio (LB3 - 20%)
- Führung eines [Lernportfolios](https://gitlab.com/ch-tbz-it/Stud/m319/-/tree/main/N0-Portfolio) in GitLab oder GitHub
- Abgabe am Tag 10

### LB1 (40%) - Tag 4
- **Dauer:** 75 Minuten
- **Inhalt:** Tag 1 bis Tag 3
- **Lernziele:** Recap M162, DBMS, General/Spezial, Non-/Identifying, DDL, DML, DCL
- **Format:** 
  - 30 min Theorie auf Papier "closed book"
  - 45 min Praxis "open book" mit Laptop

### LB2 (40%) - Tag 10
- **Dauer:** 110 Minuten
- **Inhalt:** Tag 1 bis Tag 9
- **Lernziele:** DDL, DML, DCL, Mengenlehre, Konsistenz und ref.Integrität, Beziehunges-Constraints, Aggregationsfunktionen
- **Format:**
  - 30 min Theorie auf Papier "closed book"
  - 70 min Praxis "open book" mit Laptop

---

## Detaillierte Kursübersicht

| Tag | Datum  | Kompetenzmatrix | Themen & Inhalte | Materialien |
|-----|--------|-----------------|------------------|-------------|
| 1   | 18.02. | A1              | **Einführung & Grundlagen:**<br>- Einführung in die Klasse und das Modul<br>- Auffrischen von Fachbegriffen und Konzepten<br>- Normalisieren<br>- DBMS MySQL/MariaDB Installation<br>- ERM, ERD (1.NF, 2.NF, 3.NF) am Beispiel 'Tourenplaner' | [1.Tag](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/1.Tag)<br>[Recap](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/1.Tag/Recap/Recap.md)<br>[XAMPP Installation](https://gitlab.com/ch-tbz-it/Stud/m164/-/tree/main/1.Tag/XAMPP)<br>[Docker Setup](https://gitlab.com/ch-tbz-it/Stud/m164/-/tree/main/1.Tag/Docker)<br>[AWS Cloud](https://gitlab.com/ch-tbz-it/Stud/m164/-/tree/main/1.Tag/AWSCloud)<br>[MySQL Workbench](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/1.Tag/Installation_SW.md)<br>[Tourenplaner](https://gitlab.com/ch-tbz-it/Stud/m164/-/tree/main/1.Tag/Tourenplaner) |
| 2   | 25.02. | A1, B1          | **ERD & Datenbankmodellierung:**<br>- ERD erweitern<br>- DBMS und Datenbank erstellen<br>- Generalisierung/Spezialisierung (is_a-Beziehung)<br>- Identifizierende & nicht-identifizierende Beziehungen<br>- Einführung in DDL<br>- Workbench Forward Engineering | [2.Tag](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/2.Tag)<br>[Generalisierung & Spezialisierung](https://gitlab.com/ch-tbz-it/Stud/m164/-/tree/main/2.Tag#generalisierung--spezialisierung-person-mit-der-rolle-als-fahrer-oder-disponent)<br>[DDL Intro](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/2.Tag/DDL_Intro.md) |
| 3   | 04.03. | B2, B3          | **Datentypen & Beziehungen:**<br>- Datentypen in MySQL<br>- Mehrfachbeziehungen<br>- Rekursive Beziehungen<br>- Datenbasis bearbeiten<br>- Spezielle Beziehungen<br>- DML (Data Manipulation Language) | [3.Tag](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/3.Tag) |
| 4   | 11.03. | B2, B3, C1, C3, D1 | **LB1 (40%) + Referenzielle Integrität:**<br>- Prüfung LB1<br>- Referenzielle Integrität / FK-Constraints<br>- Mengenlehre<br>- DML (JOIN-Operationen) | [4.Tag](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/4.Tag) |
| 5   | 18.03. | C1, C3, D1      | **Datenintegrität & Abfragen:**<br>- Datenintegrität<br>- DQL (Data Query Language)<br>- DCL (Data Control Language)<br>- FK-Constraint-Option Regeln<br>- SELECT-Anweisungen mit WHERE (WGHOL) | [5.Tag](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/5.Tag)<br>[SELECT Klauseln Merksatz](https://www.informatikzentrale.de/select-klauseln-merksatz.html) |
| 6   | 25.03. | C2, C3          | **Unterabfragen & Datenim-/export:**<br>- Unterabfragen (SubQueries)<br>- Massenimport von Daten (Bulkimport)<br>- Sub-SELECT<br>- LOAD DATA INFILE | [6.Tag](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/6.Tag) |
| 7   | 01.04. | C2              | **Backup & Datenintegration:**<br>- Datensicherung (Backup)<br>- Daten normalisiert einbinden<br>- Dump erstellen und verwenden<br>- Backuptools kennenlernen | [7.Tag](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/7.Tag) |
| 8   | 08.04. | A1, B1, C2      | **Praxisarbeit:**<br>- CSV-Daten in normalisierte Datenbank (3-NF) importieren<br>- OpenData verwenden | [8.Tag](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/8.Tag) |
| 9   | 15.04. | D1              | **Erweiterte Konzepte:**<br>- Common Table Expressions (CTE)<br>- Stored Procedures<br>- Praxisarbeit fortsetzen<br>- Repetitionen zur LB2 | [9.Tag](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/9.Tag) |
| 10  | 06.05. |                 | **LB2 (40%) + LB3 (20%):**<br>- Prüfung LB2<br>- Abgabe Lernjournal/Dossier LB3 | |

---

## Persönlicher Unterrichtsverlauf

### Tag 1 (18.02.2025)
- 8:10-8:50 (40 Min): Einführung ins Modul
- 8:50-9:10 (20 Min): XAMPP Installation
- 9:10-9:30 (20 Min): Konzeptentwicklung Routenplaner
- 9:30-10:50 (80 Min): ERM und ERD entwickeln
- 10:50-11:30 (40 Min): Daten extrahieren und normalisieren

### Tag 2 (25.02.2025)
- 8:10-8:40 (30 Min): Einführung in die Themen des Tages
- 8:40-9:30 (50 Min): Notizen erstellen zu den Konzepten
- 9:30-10:50 (80 Min): Schema übertragen in Workbench
- 10:50-11:30 (40 Min): Praktische Tests in phpMyAdmin

### Tag 5 (18.03.2025)
- WGHOL-Konzept kennengelernt (**W**arum **G**eht **H**erbert **O**ft **L**aufen?)
- Aggregatsfunktionen durchgearbeitet

### Tag 6 (25.03.2025)
- Kommandozeilen-Zugriff auf Datenbank eingerichtet
- Mit CRUD-Operationen und Dumps experimentiert
- Gitlab-Repository durchgearbeitet

### Tag 7 (01.04.2025)
- Über Backup-Strategien und Dumps informiert
- Daten normalisiert einbinden geübt
- Notizen erstellt und Material zusammengefasst

### Tag 8 (08.04.2025)
- CSV-Dateien importieren gelernt
- Wiederholung der Normalisierungsformen
- Vorbereitung auf die kommende Prüfung

---

## Wichtige SQL-Konzepte

### WGHOL - Ausführungsreihenfolge von SQL-Befehlen
**W**arum **G**eht **H**erbert **O**ft **L**aufen?
1. **W**HERE: Filterung der Datensätze
2. **G**ROUP BY: Gruppierung der Daten
3. **H**AVING: Filterung der gruppierten Daten
4. **O**RDER BY: Sortierung der Ergebnisse
5. **L**IMIT: Begrenzung der Anzahl der Ergebnisse

### Aggregatsfunktionen
- COUNT(): Zählt die Anzahl der Zeilen
- SUM(): Summiert numerische Werte
- AVG(): Berechnet den Durchschnitt
- MIN(): Findet den kleinsten Wert
- MAX(): Findet den größten Wert

### Beziehungstypen
- **Identifizierende Beziehung**: Der Primärschlüssel einer übergeordneten Entität wird Teil des Primärschlüssels der untergeordneten Entität
- **Nicht-identifizierende Beziehung**: Der Primärschlüssel einer übergeordneten Entität wird als Fremdschlüssel in der untergeordneten Entität verwendet, aber nicht als Teil des Primärschlüssels
- **Generalisierung/Spezialisierung**: Eine is_a-Beziehung, bei der eine allgemeine Entität (z.B. Person) spezifischere Untertypen hat (z.B. Fahrer, Disponent)

### Normalisierungsformen
1. **1. Normalform (1NF)**: Jedes Attribut enthält nur atomare Werte
2. **2. Normalform (2NF)**: Erfüllt 1NF und alle Nicht-Schlüsselattribute sind funktional vom gesamten Primärschlüssel abhängig
3. **3. Normalform (3NF)**: Erfüllt 2NF und keine transitiven Abhängigkeiten nicht-primärer Attribute vom Primärschlüssel

---

## Prüfungsvorbereitung

### LB1 Zusammenfassung (Tag 1-3)
- **Theorie (30 Min)**: Recap M162, DBMS-Grundlagen, Generalisierung/Spezialisierung, Identifying/Non-Identifying Beziehungen, DDL, DML, DCL
- **Praxis (45 Min)**: Anwendung der theoretischen Konzepte mit dem DBMS

### LB2 Zusammenfassung (Tag 1-9)
- **Theorie (30 Min)**: Alle Konzepte aus LB1 plus Mengenlehre, Konsistenz und referentielle Integrität, Beziehungs-Constraints, Aggregatsfunktionen
- **Praxis (70 Min)**: Daten in 3-NF-Datenbasis einbinden, auslesen und sichern
