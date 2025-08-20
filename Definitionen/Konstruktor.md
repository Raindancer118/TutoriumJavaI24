---
aliases:
  - Konstruktoren
---
# Konstruktor
Der Konstruktor ist eine [[Methode]], die in der [[Klasse]] steht und dafür verantwortlich ist, [[Objekt|Objekte]] der [[Klasse]] zu erzeugen. Er bietet außerdem die Möglichkeit, [[Parameter]] bei einer Objekterstellung mitzugeben, sodass der Anfangszustand des [[Objekt|Objektes]] festgelegt werden kann.
## Eigenschaften
- Der Konstruktor hat **immer denselben Namen** wie seine [[Klasse]] selbst.
- Ein Konstruktor **kann** keinen [[Datentypen|Rückgabewert]] haben, auch **kein void**.
- Sollte es keinen Konstruktor geben, fügt der Compiler einen **parameterlosen Standardkonstruktor** ein.

>[!HINT] Eine Klasse kann mehrere Konstruktoren haben.
>Dies nennt man dann **Überladung**.

## Aufruf
Der Konstruktor einer Klasse wird mit dem Aufruf `new [Klassenname]`aufgerufen.

>[!EXAMPLE]
>```
>Auto audi = new Auto("Audi");
>``` 
## Aufbau
Für den Aufbau wird zunächst der Sichtbarkeitsmodifikator des Konstruktors gesetzt. Dieser bestimmt in diesem Fall, ob [[Objekt|Objekte]] der Klasse aus dem eigenen Package oder auch von außerhalb erstellt werden dürfen.
Anschließend steht der Name der Klasse. 
Daraufhin folgt die Parameterliste. Die beiden runden Klammern müssen auch dann leer hingeschrieben werden, wenn es keine [[Parameter]] für den Konstruktor gibt. 

>[!EXAMPLE]
>```
>public Auto (String marke) {}
>```
