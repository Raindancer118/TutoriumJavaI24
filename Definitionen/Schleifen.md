# Schleifen
Es gibt vor allem zwei sehr große Schleifentypen, die ich hier gern erläutern möchte. Diese habt ihr auch beide in der Vorlesung gemacht.

Alle Schleifen können über **break;** verlassen werden.
## [[Foliensatz03.pdf#page=8|While]]
Es gibt zwei verschiedene Arten von While-Schleifen. Sie unterscheiden sich hierbei nicht nur darin, wo das "while" steht, sondern auch darin, wie oft und unter welcher Bedingung die Schleife ausgeführt wird.
### do ... while (do-Schleife)
Die Do-Schleife wird auch **nicht abweisende Schleife** genannt. Dies liegt daran, dass die Ausführung der Schleife vor ihrer Bedingung passiert. Somit wird auch bei nichtzutreffender Bedingung die Anweisung der Schleife einmal ausgeführt.
>[!Syntax]
>```
>do { ...
>... } while ([bedingung]);
>```

### while ... do (while-Schleife)
Die **While-Schleife** ist die **abweisende** Schleife. Diese Benennung liegt daran, dass die Anweisung in der Schleife nur bei zutreffender Bedingung ausgeführt wird. 
>[!Syntax]
>```
>while ([bedingung]) {
>... }
>```

## For (For Each-Schleife)
Die For Each Schleife wird auch als **Zählende Schleife** bezeichnet.