Die SQL-Befehle WHERE,
GROUP BY, 
HAVING, ORDER BY und LIMIT werden verwendet, 
um Daten aus einer Datenbank abzurufen und zu filtern. 
Hier ist eine kurze Zusammenfassung ihrer Funktionen und Reihenfolge:

WHERE:

Filtert die Zeilen, bevor die Gruppierung oder Aggregation erfolgt.

Beispiel: SELECT * FROM Kunden WHERE Land = 'Deutschland';
GROUP BY:

Gruppiert die Daten basierend auf einer oder mehreren Spalten.

Beispiel: SELECT Land, COUNT(*) FROM Kunden GROUP BY Land;
HAVING:

Filtert Gruppen nach einer Bedingung, wird nach GROUP BY angewendet.
Beispiel: SELECT Land, COUNT(*) FROM Kunden GROUP BY Land HAVING COUNT(*) > 5;
ORDER BY:

Sortiert die Ausgabe nach einer oder mehreren Spalten, aufsteigend (ASC, Standard) oder absteigend (DESC).

Beispiel: SELECT * FROM Kunden ORDER BY Name DESC;
LIMIT:

Begrenzung der Anzahl der zurückgegebenen Zeilen.

Beispiel: SELECT * FROM Kunden ORDER BY Name LIMIT 10;

Reihenfolge der Ausführung in SQL:
FROM (Tabelle auswählen)
WHERE (Zeilen filtern)
GROUP BY (Gruppieren)
HAVING (Gruppen filtern)
SELECT (Spalten auswählen)
ORDER BY (Sortieren)
LIMIT (Ergebnis begrenzen)

Aggregatsfunktionen in Datenbanken ermöglichen es, Berechnungen über eine Menge von Zeilen durchzuführen und liefern einen einzelnen Wert als Ergebnis. Die gängigsten Aggregatsfunktionen sind:

- **`COUNT()`**: Zählt die Anzahl der Zeilen in einer Ergebnismenge.
- **`SUM()`**: Summiert die Werte einer bestimmten Spalte.
- **`AVG()`**: Berechnet den Durchschnittswert einer Spalte.
- **`MIN()`**: Gibt den kleinsten Wert einer Spalte zurück.
- **`MAX()`**: Gibt den größten Wert einer Spalte zurück.

**Beispiele:**

1. **`COUNT()`**: Um die Anzahl der Mitarbeiter in einer Tabelle `employees` zu ermitteln:

   ```sql
   SELECT COUNT(*) FROM employees;
   ```


2. **`SUM()`**: Um die Gesamtsumme der Gehälter zu berechnen:

   ```sql
   SELECT SUM(salary) FROM employees;
   ```


3. **`AVG()`**: Um das durchschnittliche Gehalt zu ermitteln:

   ```sql
   SELECT AVG(salary) FROM employees;
   ```


4. **`MIN()`** und **`MAX()`**: Um das niedrigste und höchste Gehalt zu finden:

   ```sql
   SELECT MIN(salary) AS niedrigstes_gehalt, MAX(salary) AS hoechstes_gehalt FROM employees;
   ```


**Hinweise:**

- Aggregatsfunktionen ignorieren in der Regel NULL-Werte.
- Sie können mit der `GROUP BY`-Klausel kombiniert werden, um Aggregationen für Gruppen von Zeilen durchzuführen.

**Beispiel mit `GROUP BY`:**

Um die durchschnittlichen Gehälter pro Abteilung zu berechnen:


```sql
SELECT department, AVG(salary) FROM employees GROUP BY department;
```


Dieses Statement liefert das durchschnittliche Gehalt für jede Abteilung.

Für weitere Details und spezifische Beispiele empfehle ich, die bereitgestellten Materialien unter dem angegebenen Link zu konsultieren. 
