# Lernjournal
___
**Quellen**:

TBZ:
https://gitlab.com/harald.mueller/aktuelle.kurse/-/tree/master/m164

Internet:

NY:

sonstige:
[Modulbaukasten](https://www.modulbaukasten.ch/module/164/1/de-DE?title=Datenbanken-erstellen-und-Daten-einf%C3%BCgen)

___
## Inhaltsverzeichnis:


___


## Leistungsbeurteilungen (Prüfungen)

- Sie führen in diesem Modul ein [Lernportfolio](https://gitlab.com/ch-tbz-it/Stud/m319/-/tree/main/N0-Portfolio).  
    Vorzugsweise in GitLab oder GitHub. Die Bewertung ist Teil der **LB3**.  
      
    
- Am Tag 4 **LB1 (40%)** 75 min mit Inhalt von Tag 1 bis Tag 3  
    (Lernziele: Recap M162, DBMS, General/Spezial, Non-/Identifying, DDL, DML, DCL)  
    30 min Theorie auf Papier "closed book" plus 45 min "open book" mit Laptop (Praxis)  
      
    
- Am Tag 10 **LB2 (40%)** 110 min mit Inhalt von Tag 1 bis Tag 9  
    (Lernziele: DDL, DML, DCL, Mengenlehre, Konsistenz und ref.Integrität, Beziehunges-Constraints, Aggregationsfunktionen, "alles")  
    30 min Theorie auf Papier "closed book" plus 70 min "open book" mit Laptop (Praxis)  
      
    
- Am Tag 10 **LB3 (20%)** die [Abgabe des Lern-Portfolios](https://gitlab.com/ch-tbz-it/Stud/m319/-/tree/main/N0-Portfolio)

*Quelle: Harald Müller*
___

## Ablaufplan 2024/25-Q3 **AP24a** (Di morgens)

| Tag | Datum  | [KmpMatrx](https://gitlab.com/modulentwicklungzh/cluster-data/m164/-/tree/master/1_Kompetenzmatrix?ref_type=heads) | Thema, Auftrag, Übung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | Check |
| --- | ------ | ------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----- |
| 1   | 18.02. | A1                                                                                                                 | [Einführung, Auffrischen Fachbegriffe, Konzepte, Normalisieren](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/1.Tag)  <br>[Recap](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/1.Tag/Recap/Recap.md)  <br>DBMS MySQL/MariaDB installieren: (service/deamon & client) ([Xampp](https://gitlab.com/ch-tbz-it/Stud/m164/-/tree/main/1.Tag/XAMPP), [Docker](https://gitlab.com/ch-tbz-it/Stud/m164/-/tree/main/1.Tag/Docker), [AWS cloud](https://gitlab.com/ch-tbz-it/Stud/m164/-/tree/main/1.Tag/AWSCloud), [MySqlWorkbench](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/1.Tag/Installation_SW.md) )  <br>[ERM, ERD (1.NF, 2.NF, 3.NF) am Bsp. 'Tourenplaner'](https://gitlab.com/ch-tbz-it/Stud/m164/-/tree/main/1.Tag/Tourenplaner) |       |
| 2   | 25.02. | A1, B1                                                                                                             | [ERD erweitern, DBMS, Datenbank erstellen](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/2.Tag)  <br>Generalisierung / Spezialisierung ([is_a-Beziehung](https://gitlab.com/ch-tbz-it/Stud/m164/-/tree/main/2.Tag#generalisierung--spezialisierung-person-mit-der-rolle-als-fahrer-oder-disponent)), [indentifizierende & nicht-identifizierende Beziehungen](https://www.datenbank-grundlagen.de/beziehungen-datenbanken.html)  <br>[Einführung in DDL](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/2.Tag/DDL_Intro.md)  <br>Workbench Forward Engineering → DDL (CHARSET)                                                                                                                                                               |       |
| 3   | 04.03. | B2, B3                                                                                                             | [Datentypen, Mehrfachbeziehungen, Rekursion, Datenbasis bearbeiten, Spezielle Beziehungen, DML](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/3.Tag)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |       |
| 4   | 11.03. | B2, B3, C1, C3, D1                                                                                                 | **LB1 (40%)**  <br>  <br>[Ref. Integrität / FK-Constraints, Mengenlehre, DML (JOIN)](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/4.Tag)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |       |
| 5   | 18.03. | C1, C3, D1                                                                                                         | [Datenintegrität, DQL, DCL](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/5.Tag) FK-Constraint-Option Regeln  <br>SELECT ... WHERE ... ([**W**arum **G**eht **H**erbert **O**ft **L**aufen?](https://www.informatikzentrale.de/select-klauseln-merksatz.html))                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |       |
| 6   | 25.03. | C2, C3                                                                                                             | [SubQueries, Bulkimport](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/6.Tag) Sub-SELECT, LOAD DATA INFILE                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |       |
| 7   | 01.04. | C2                                                                                                                 | [Backup, Daten normalisiert einbinden](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/7.Tag) Dump erstellen und Backuptool  <br>Daten in normalisierte DB importieren                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |       |
| 8   | 08.04. | A1, B1, C2                                                                                                         | [Praxisarbeit](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/8.Tag) zum Üben - CSV-Data → DB-3.NF OpenData                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |       |
| 9   | 15.04. | D1                                                                                                                 | [Common Table Expressions & Stored Procedures](https://gitlab.com/ch-tbz-it/Stud/m164/-/blob/main/9.Tag)  <br>Weitermachen am Praxisarbeit und Repetitionen zur LB2                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |       |
| --  | ----   |                                                                                                                    | Osterferien                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |       |
| 10  | 06.05  |                                                                                                                    | **LB2 (40%)** und  <br>Abgabe Lernjournal/Dossier **LB3 (20%)**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |       |
*Quelle: Harald Müller*
___



Ablauf
___

18.02.2025

- 8:10-8:50 (40) Einführung
- 8:50-9:10(20) XAMP Instalieren
- 9:10-0:00() Routenplaner auftrag
- 9:10-9:30(20) Konzept
- 9:30-10:50(80) ERM und ERD
- 10:50-11:30(40)Daten Extrahiert normalisiert

___
25.02.2025

- 8:10-8:40 (30) Einführung
- 8:40-9:30(50) Notizen erstellen
- 9:30-10:50(80) Schema übertragen
- 10:50-11:30(40) Auf PHPAdmin ausprobiert
  
___
18.03.2025

-WGHOL angeschaut



