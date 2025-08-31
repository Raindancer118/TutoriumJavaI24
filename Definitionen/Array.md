# Array
Ein Array ist eine besondere Art von [[Sammlung]], die eine festgelegte Anzahl von Elementen halten kann.
## Eigenschaften
- Arrays haben **immer eine feste Größe**. Diese wird bei der Erstellung festgelegt und kann später nicht mehr verändert werden.
- Jedes Element im Array hat denselben [[Datentyp]].
- Die Elemente sind **nummeriert** (Index beginnt bei `0` und geht bis `length-1`).
- Arrays sind [[Objekt|Objekte]], besitzen aber **keine eigenen Methoden** – nur die Eigenschaft `.length`.
- Sie können sowohl [[primitive Datentypen]] als auch Objekte speichern.
## Aufbau

Ein Array durchläuft drei Schritte:
1. **Deklaration** einer Array-Variable
2. **Erstellung** eines Arrays mit `new`
3. **Verwendung** durch Zugriff auf die Indices
## Zugriff

- Elemente werden mit `[]` angesprochen (`zahlen[0]`).
- Mit einer [[for-Schleife]] oder [[for-each-Schleife]] können Arrays durchlaufen werden.

```
// Deklaration und Erstellung
int[] zahlen = new int[5];

// Initialisierung
zahlen[0] = 42;
zahlen[1] = 17;

// Direktes Initialisieren
String[] namen = {"Alice", "Bob", "Charlie"};

// Zugriff und Ausgabe
System.out.println(zahlen[0]); // 42

// Länge des Arrays
System.out.println("Anzahl: " + zahlen.length);

// Iteration mit for-each
for (String name : namen) {
   System.out.println(name);
}
```
