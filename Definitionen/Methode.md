---
aliases:
  - Methoden
  - Verhalten
---
# Methode
Eine Methode ist eine einzelne Funktion einer [[Klasse]]. Alle Methoden einer [[Klasse]] gemeinsam bestimmen ihr Verhalten.

## Aufbau
Eine Methode beginnt mit der **Methodensignatur**. Diese setzt sich zusammen aus dem Zugriffsmodifikator, den die Methode haben soll, dem [[Datentypen|Rückgabetypen]], also dem [[Datentypen|Datentyp]], den die Methode zurückgeben soll, dem Methodenname und der Parameterliste, also einer Auflistung aller [[Parameter]], die bei Aufruf der Methode mitgegeben werden müssen.

>[!Example]
>Hier eine beispielhafte Methodensignatur:
>```
>public void streicheln(hund hund) {
>```
>Die hier gegebene Methode hat folgende Eigenschaften:
>- Sichtbarkeitsmodifikator *public* - Die Methode auch außerhalb des eigenen Packages sichtbar
>- Rückgabetyp *void* - Die Methode gibt keine Daten zurück
>- Methodenname *streicheln*
>- [[Parameter]] *hund hund* - Es soll offensichtlich ein [[Objekt]], das in der Methode als *hund* bezeichnet wird, vom [[Datentypen|Typ]] *hund* mitgegeben werden.

>[!HINT]
>Nach einem **return**-Statement wird eine Methode **immer** verlassen. Return Statements können auch dann in die Methode eingefügt werden, wenn diese keinen [[Datentypen|Rückgabetypen]] hat. Es muss hierbei nur darauf geachtet werden, dass hinter dem return keine Variable oder Daten stehen.
