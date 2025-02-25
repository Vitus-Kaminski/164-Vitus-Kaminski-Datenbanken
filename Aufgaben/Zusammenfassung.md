**Generalisierung und Spezialisierung in der Datenbankmodellierung**

In der Datenbankmodellierung begegnen wir oft dem Problem, dass mehrere Entitätstypen viele gemeinsame Attribute haben, jedoch auch spezifische Merkmale besitzen. Dies kann zu Redundanz führen, wenn dieselben Attribute in mehreren Tabellen gespeichert werden. Eine effiziente Lösung besteht in der **Generalisierung** und **Spezialisierung**:

- **Generalisierung:** Gemeinsame Attribute werden in einem allgemeinen Entitätstyp zusammengefasst. Beispielsweise könnte eine allgemeine "Person"-Tabelle Attribute wie Name, Geburtsdatum und Telefonnummer enthalten, die sowohl für Mitarbeiter als auch für Kunden gelten.
- **Spezialisierung:** Spezifische Attribute bleiben in den spezialisierten Tabellen. Beispielsweise könnten Fahrer eine "Fahrerlaubnis" und Disponenten eine "Planungskompetenz" als Attribute haben.
- **IS_A-Beziehung:** Die spezialisierten Tabellen verweisen per Fremdschlüssel auf die generalisierte Tabelle, um eine konsistente Datenstruktur zu gewährleisten.

**Beispiel:**
- Eine "Person"-Tabelle enthält allgemeine Attribute (Name, Adresse, Geburtsdatum).
- Eine "Mitarbeiter"-Tabelle verweist auf "Person" und enthält zusätzliche Attribute wie Gehalt.
- Eine "Kunde"-Tabelle verweist ebenfalls auf "Person" und enthält Attribute wie Kundenstatus.

---

**Identifying und Non-Identifying Relationships**

Datenbankbeziehungen lassen sich in zwei Hauptkategorien unterteilen:

- **Identifying Relationship:** Der Fremdschlüssel ist ein Teil des Primärschlüssels der untergeordneten Tabelle. Diese Beziehung sorgt für eine enge Kopplung der Datensätze. Beispiel: Ein Raum existiert nur innerhalb eines Gebäudes und hat als Primärschlüssel eine Kombination aus Raum-ID und Gebäude-ID.
- **Non-Identifying Relationship:** Der Fremdschlüssel ist kein Teil des Primärschlüssels der untergeordneten Tabelle. Diese Beziehung erlaubt mehr Flexibilität, da der Fremdschlüssel geändert werden kann. Beispiel: Ein Mitarbeiter gehört zu einer Abteilung, kann jedoch in eine andere Abteilung wechseln, ohne dass sich seine Mitarbeiter-ID ändert.

**Beispiele:**
- **Identifying Relationship:** Ein Student ist einer Universität zugeordnet. Die Student-ID enthält die Universität-ID.
- **Non-Identifying Relationship:** Ein Lehrer unterrichtet verschiedene Klassen, aber seine Lehrer-ID bleibt gleich.

---

**Datenbankmanagementsystem (DBMS)**

Ein **DBMS (Datenbankmanagementsystem)** ist eine Software zur Speicherung, Verwaltung und Abfrage von Daten in einer strukturierten Weise.

**Merkmale eines DBMS:**
- **Integrierte Datenhaltung:** Vermeidung von Redundanz durch zentrale Datenverwaltung.
- **Datenbanksprache:** Ermöglicht Datenabfragen (DQL), Definition (DDL), Manipulation (DML) und Berechtigungssteuerung (DCL).
- **Mehrbenutzerfähigkeit:** Synchronisation von konkurrierenden Transaktionen.
- **Konsistenzkontrolle:** Sicherstellung der Integrität der Daten.
- **Transaktionen:** Verwaltung von Datenbankänderungen als atomare Einheiten.
- **Datenzugriffskontrolle:** Schutz sensibler Daten durch Benutzerrechte.

**Vorteile eines DBMS:**
- Hohe Datenverfügbarkeit und Sicherheit
- Effiziente Speicherung und Abfrage von Daten
- Flexibilität bei sich ändernden Anforderungen
- Kürzere Entwicklungszeiten für Anwendungen

**Beispiele für bekannte DBMS:**
- **Relationale DBMS:** MySQL, PostgreSQL, MS SQL Server, Oracle
- **Objektrelationale DBMS:** IBM DB2, Informix
- **NoSQL-Datenbanken:** MongoDB, Cassandra

---

**Zusammenfassung SQL-Befehle (DDL)**

**Datenbank anlegen:**
```sql
CREATE DATABASE db_example CHARACTER SET utf8mb4;
```

**Tabelle erstellen:**
```sql
CREATE TABLE tbl_mitarbeiter (
    MA_ID INT PRIMARY KEY,
    Name VARCHAR(50) CHARACTER SET latin1,
    Vorname VARCHAR(30) CHARACTER SET latin1,
    Geburtsdatum DATETIME,
    Telefonnummer VARCHAR(12),
    Einkommen FLOAT(10,2)
);
```

**Tabelle ändern:**
```sql
ALTER TABLE tbl_mitarbeiter MODIFY Name VARCHAR(50) CHARACTER SET utf8mb4;
```

**Tabelle löschen:**
```sql
DROP TABLE tbl_mitarbeiter;
```


