**Zusammenfassung: Datensicherung von Datenbanken**

Datenbanksysteme sind essenziell für Websites und Unternehmen, da sie Daten speichern und bereitstellen. Ein Datenverlust, sei es durch technische Fehler oder Benutzerfehler, kann schwerwiegende Konsequenzen haben. Um dem entgegenzuwirken, sind regelmässige Backups erforderlich.

### **Arten der Datensicherung**

1. **Online-Backup**: Die Datenbank bleibt während des Backups aktiv, wodurch sie weiterhin nutzbar ist.
    
2. **Offline-Backup**: Die Datenbank wird während des Backups heruntergefahren, was eine höhere Datensicherheit bietet, jedoch zu Ausfallzeiten führt.
    

**Backup-Methoden:**

- **Voll-Backup**: Speichert alle Daten, benötigt viel Speicherplatz, ist aber für eine einfache Wiederherstellung geeignet.
    
- **Differentielles Backup**: Sichert nur Änderungen seit dem letzten Voll-Backup. Spart Speicherplatz, erfordert aber mehrere Dateien zur Wiederherstellung.
    
- **Inkrementelles Backup**: Sichert nur Änderungen seit dem letzten Backup (egal ob Voll- oder inkrementell), minimiert Speicherbedarf, benötigt jedoch alle vorherigen Sicherungen für eine Wiederherstellung.
    

### **Tools zur Datensicherung**

- **MySQLDump**: Bietet eine schnelle Sicherung und Wiederherstellung über die Kommandozeile.
    
- **phpMyAdmin**: Erlaubt den Export von SQL-Datenbanken, jedoch mit Speicherlimitierungen.
    
- **BigDump**: Kann grosse Backups einspielen, hat aber keine eigene Sicherungsfunktion.
    
- **HeidiSQL**: Backup-Tool für Windows, jedoch ohne Automatisierungsoption.
    
- **Mariabackup**: Open-Source-Tool zur Erstellung physischer Backups von MariaDB-Tabellen.
    

### **Backup-Sicherheit**

- Backups sollten auf externen Medien gespeichert werden.
    
- Daten sollten verschlüsselt werden, um Missbrauch zu verhindern.
    
- Sicherungskopien sollten an verschiedenen Orten aufbewahrt werden.
    

---

**Fragen und Antworten:**

1. **Grundsätzlicher Ablauf zur Normalisierung einer DB:**
    
    - Erste Normalform (1NF): Aufteilung der Tabellen in atomare Felder.
        
    - Zweite Normalform (2NF): Trennung von Daten mit Abhängigkeiten.
        
    - Dritte Normalform (3NF): Entfernung aller nicht-schlüsselabhängigen Attribute.
        
2. **Unterschied zwischen logischem und physischem Backup:**
    
    - Logisches Backup: Exportiert Daten als SQL-Skripte (z. B. MySQLDump).
        
    - Physisches Backup: Kopiert direkt die Dateien der Datenbank.
        
3. **Restore-Prozess der Backup-Typen:**
    
    - **Voll-Backup**: Direktes Einspielen der gesamten Sicherung.
        
    - **Inkrementelles Backup**: Wiederherstellung erfolgt durch das letzte Voll-Backup + alle inkrementellen Backups.
        
    - **Differentielles Backup**: Wiederherstellung durch das letzte Voll-Backup + das neueste differenzielle Backup.
        
4. **Drei Möglichkeiten, eine Datenbank zu sichern:**
    
    - **MySQLDump:** `mysqldump -u Benutzer -p Datenbankname > backup.sql`
        
    - **phpMyAdmin:** Exportfunktion nutzen.
        
    - **Mariabackup:** `mariabackup --backup --target-dir=/backup/path`
        
5. **Fünf Schritte zur 3. Normalform:**
    
    - 1NF: Entfernen redundanter Gruppen.
        
    - 2NF: Sicherstellen, dass alle Attribute von der Primärschlüssel abhängen.
        
    - 3NF: Entfernen von Abhängigkeiten, die nicht von der Schlüsselabhängigkeit stammen.
        
    - Identifikation von Beziehungen zwischen Tabellen.
        
    - Sicherstellung der Integrität mit Fremdschlüsseln.
        
6. **Befehl SELECT INTO OUTFILE:**
    
    - `SELECT * FROM Tabelle INTO OUTFILE '/pfad/zu/datei.csv' FIELDS TERMINATED BY ',';`
        
    - Exportiert das Abfrageergebnis in eine Datei.
        
