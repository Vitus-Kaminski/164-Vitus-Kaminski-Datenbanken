**Zusammenfassung: Identifying und Non-Identifying Relationships**

In relationalen Datenbanken unterscheidet man zwischen **Identifying** und **Non-Identifying Relationships**. Diese Beziehungen definieren, wie Entitäten miteinander verknüpft sind und ob der Fremdschlüssel Teil des Primärschlüssels ist.

### **1. Identifying Relationship**
Bei einer Identifying Relationship ist der Fremdschlüssel **Teil des Primärschlüssels** der abhängigen (Kind-)Tabelle. Dadurch wird sichergestellt, dass die untergeordnete Entität ohne die übergeordnete nicht existieren kann.

#### **Beispiel:**
- **Person → Ausweis**
  - Eine Person kann mehrere Ausweise besitzen.
  - Die **Ausweisnummer** allein reicht nicht zur Identifikation aus, sie muss in Kombination mit der **Personen-ID** als Primärschlüssel dienen.
  - **Primärschlüssel von "Ausweis" = (Personen-ID, Ausweisnummer)**.

### **2. Non-Identifying Relationship**
Bei einer Non-Identifying Relationship ist der Fremdschlüssel **kein Bestandteil des Primärschlüssels** der abhängigen Tabelle. Diese Beziehung erlaubt, dass die untergeordnete Entität unabhängig von der übergeordneten existiert.

#### **Beispiel:**
- **Person → Kleidungsstück**
  - Eine Person kann mehrere Kleidungsstücke besitzen, aber die Kleidungsstücke existieren unabhängig von einer spezifischen Person.
  - Die **Kleidungsstück-ID** ist der Primärschlüssel der Tabelle "Kleidungsstück", während die **Personen-ID** nur als Fremdschlüssel gespeichert wird.

---

### **Eigene Generalisierung**
Ein Beispiel für eine Generalisierung wäre die Entität "Fahrzeug" mit den spezialisierten Entitäten "Auto" und "Motorrad".

- **Superklasse:** Fahrzeug (enthält gemeinsame Attribute wie "Fahrzeugnummer" und "Hersteller").
- **Subklassen:** Auto (zusätzliche Attribute wie "Anzahl Türen") und Motorrad (zusätzliche Attribute wie "Hubraum").

---

### **Beispiele von Klassenkameraden:**
- **Buch → Kapitel** (Identifying Relationship, da Kapitel nicht ohne Buch existiert).
- **Schule → Schüler** (Non-Identifying Relationship, da Schüler unabhängig von einer Schule existieren können).

---

### **Anwendungsfälle für Identifying Relationships**
1. **Bestellungen und Bestellpositionen**: Eine Bestellposition existiert nur innerhalb einer Bestellung.
2. **Flugzeuge und Sitze**: Ein Sitz existiert nur in einem bestimmten Flugzeug.
3. **Projekte und Aufgaben**: Eine Aufgabe gehört zu genau einem Projekt und existiert nicht unabhängig.

---

### **DBMS – Datenbank-Management-System**
Ein **DBMS** ist ein System zur Verwaltung großer Datenmengen. Es sorgt für effiziente Speicherung, Konsistenz und Zugriffskontrolle.

#### **Merkmale eines DBMS:**
- **Datenorganisation:** Strukturierte Speicherung und Verknüpfung von Daten.
- **Konsistenzkontrolle:** Sicherstellung der Datenintegrität.
- **Mehrbenutzerfähigkeit:** Gleichzeitiger Zugriff durch mehrere Benutzer.
- **Sicherheitsmechanismen:** Zugriffskontrolle und Authentifizierung.

#### **Top 10 DBMS (DB-Engines Ranking):**
1. Oracle
2. MySQL
3. Microsoft SQL Server
4. PostgreSQL
5. MongoDB
6. Redis
7. IBM Db2
8. Elasticsearch
9. SQLite
10. Snowflake

---

### **DDL – Datenbank anlegen (SQL)**
Ein Datenbankschema kann mit **DDL (Data Definition Language)** erstellt werden.

#### **Beispiel: Erstellung einer Datenbank mit MySQL**
```sql
CREATE DATABASE LernDB CHARACTER SET utf8mb4;
USE LernDB;

CREATE TABLE Person (
    PersonenID INT PRIMARY KEY,
    Name VARCHAR(50),
    Vorname VARCHAR(30)
);

CREATE TABLE Ausweis (
    Ausweisnummer INT,
    PersonenID INT,
    PRIMARY KEY (Ausweisnummer, PersonenID),
    FOREIGN KEY (PersonenID) REFERENCES Person(PersonenID)
);
```
---

### **Forward Engineering mit MySQL Workbench**
Mit **Forward Engineering** kann man aus einem Modell ein SQL-Skript generieren und automatisch eine Datenbankstruktur erstellen. Dies hilft, Fehler zu reduzieren und die Datenbank konsistent aufzubauen.

**Schritte:**
1. Datenmodell in MySQL Workbench erstellen.
2. Menü: **Database > Forward Engineer** wählen.
3. SQL-Skript generieren lassen und abspeichern.
4. Skript auf dem Datenbankserver ausführen.

---

### **Fazit**
- **Identifying Relationship**: Fremdschlüssel ist Teil des Primärschlüssels (starke Abhängigkeit).
- **Non-Identifying Relationship**: Fremdschlüssel ist nicht Teil des Primärschlüssels (flexible Beziehung).
- **DBMS** ermöglicht eine effiziente Verwaltung und Strukturierung von Daten.
- **DDL-Befehle** helfen beim Anlegen und Verwalten von Datenbanken.
- **Forward Engineering** unterstützt die Erstellung komplexer Datenbanken.



