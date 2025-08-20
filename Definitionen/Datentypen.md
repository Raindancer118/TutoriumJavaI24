---
aliases:
  - Rückgabetypen
  - Datentyp
  - Typen
  - typ
  - Rückgabewert
---
# Datentypen
## Primitiv
Es gibt in Java **acht** primitive Datentypen. Primitive Datentypen zeichnen sich dadurch aus, dass sie einen **festen Speicherbedarf** haben, der unabhängig von ihrem Inhalt immer gleich ist. Sie haben weiterhin **keine [[Methode|Methoden]]** und werden **direkt im Speicher** abgelegt.
Die primitiven Datentypen sind:

#### boolean
Eine Boolean speichert einen Wahrheitswert, also *true* oder *false*. Sie nimmt so genau ein bit ein.
```
boolean flag = true;
```
#### char
Ein char ist ein [Unicode](https://home.unicode.org/)-Zeichen und nimmt exakt 16 bit ein.
```
char letter = 'A';
```
#### byte
Ein byte ist eine *Ganzzahl zwischen -128 und +127*.
```
byte num = 100;
```
#### short
Ein short ist eine *Ganzzahl zwischen -32.768 unf 32.767*.
```
short num = 12345;
```
#### int
Eine Integer ist eine *Ganzzahl zwischen -2 Mrd und +2 Mrd*. Dabei spiegelt sie eigentlich den Standard der Datenspeicherung ab, was Zahlen angeht. 
```
int num = 42;
```
#### long
Eine Long ist eine *Ganzzahl zwischen -9 Trillionen und +9 Trillionen*. 
In der Zuweisung muss bei diesem Datentypen darauf geachtet werden, dass ans Ende der zuzuweisenden Zahl ein **L** steht.
```
long bigNum = 12345678900L;
```

#### float
Eine Float ist eine *Gleitkommazahl*. Sie hat einfache Genauigkeit. Eine Float kann ca 6-7 genaue Stellen abbilden.
In der Zuweisung muss bei diesem Datentypen darauf geachtet werden, dass statt einem Komma ein Punkt verwendet wird. Weiterhin muss ein kleines **f** an die Zahl angehängt werden.
**Float als Datentyp sollte nicht für Anwendungen verwendet werden, die mit Geld arbeiten!**
```
float pi = 3.14f;
```
#### double
Eine Double ist ebenfalls eine *Gleitkommazahl*. Sie ist doppelt so genau wie eine [[#float]]. Sie hat damit ca 15-16 genaue Stellen.
**Double als Datentyp sollte nicht für Anwendungen verwendet werden, die mit Geld arbeiten!**
```
double precisePi = 3.141592653589793;
```
## Nicht Primitiv
Nicht primitive Datentypen sind etwas abstrakter als primitive Datentypen. 
Sie unterscheiden sich von Primitiven Datentypen durch mehrere Aspekte:
- Sie können [[Methode|Methoden]] beiten
- Sie können "null" als Wert haben
Es kann sich hierbei beispielsweise handeln um:
#### [[Klasse|Klassen]]
Jede [[Klasse]] wird gleichzeitig auch ein Datentyp. Erstellte [[Objekt|Objekte]] der [[Klasse]] haben automatisch den Datentypen der [[Klasse]].
>[!EXAMPLE]
>```
>public class hund() {}
>```
>[[Objekt|Objekte]] dieser [[Klasse]] werden den Datentyp *hund* haben.

#### Interfaces
Bei Interfaces verhält es sich genau wie bei [[Klasse|Klassen]]. Siehe bitte [[#Klasse Klassen|hier]].
#### Array
#### Enum
#### Java-Bibliotheks-[[Klasse|Klassen]]
Hierbei kann es sich um [[Klasse|Klassen]] wie beispielsweise **ArrayLists** oder auch **HashMaps** handeln.
# Rückgabetypen
Alle Datentypen können auch gleichzeitig Rückgabetypen sein. Allerdings gibt es einen Rückgabetypen, der nicht konkret als Datentyp klassifiziert werden kann. Es handelt sich hierbei um:
#### void
**void** ist ein Rückgabetyp, der der [[Methode]], in die er eingesetzt ist, signalisiert, dass keine Rückgabe erwartet wird. 
Jede [[Methode]], die keine Rückgabe haben soll, **benötigt void**.